# Introduction #

Issues such as [Issue 548](https://code.google.com/p/pychess/issues/detail?id=548) and [Issue 549](https://code.google.com/p/pychess/issues/detail?id=549) have shown, that the current UI/GameModel/Engine split has much to wish for. In particular things tend to mess up when different players concurrently tries to interact with the GameModel, such as if the user undos while the engine is making a move.

A fix for this could, if not too radical, be implemented as 0.10.1 or so.

# Details #

![https://docs.google.com/drawings/pub?id=1vbpUCnhwCxGlnCxpLUcdOfGw0Sqp9TeyzjbwkSe3lqs&w=464&h=362&nonsense=something_that_ends_with.png](https://docs.google.com/drawings/pub?id=1vbpUCnhwCxGlnCxpLUcdOfGw0Sqp9TeyzjbwkSe3lqs&w=464&h=362&nonsense=something_that_ends_with.png)
[Edit](https://docs.google.com/drawings/edit?id=1vbpUCnhwCxGlnCxpLUcdOfGw0Sqp9TeyzjbwkSe3lqs&hl=en&authkey=CLeNz8IC)

## Thoughts ##

### Nonshared Gameobjects ###
Nonshared gameobjects should give less trouble with the lutils tools, which have the habit of changing the models, and not always putting them back together in the right way.
### Queues ###
The queue system reminds more of the way human people play chess. It is generally good for threaded systems to mimic real life. Further more, it allows creating "offer queues" in the fics interface for actions the user can respond to.
### Threads ###
The threads are there in ensure snappyness of the UI. By always having a ready thread in the GM and each of the engines, we assure they are always ready to handle new tasks. The requirement of rediness is also why we don't want any threads to block on Queue.get, but rather poll it.
### Messages and Intents ###
MoveIntents could all include a 'hash' (e.g. fen) of their current board state. This way the GM can be made more robust. It will however require a protocol for 'getting back on track'.
We could perhaps draw more inspiration on the UCI protocol, which tends to be less troublesome.

## Discussion ##
### Should we use processes? ###
#### Pros: ####
  * As python still have the GIL, and probably will for the foreseeable future, a process split may win us more on snappyness than threads.
  * Processes have higher promises of isolating things.
#### Cons: ####
  * Due to engines being in processes, we already utilize most cpus out there.
  * A process split will require the PyChess lib to be reimportet by each actor, and thus require more ram.
  * There might be some important shared stuff, we just havent thought about yet?

### Initing objects ###
The new more 'alive' objects for Engines and GM can result in problems for the initializing code. If the actors start acting as soon as you create them, they will be harder to configure and negotiate about.

#### Using states ####
The problem could be solved by letting the objects have a nonrunning prestate. In this state their GameState wouldn't be imutable and generally they would be more open to suggestions.
Unfortunately, this may create very complex objects. The UCIEngine is a failed example on this idea.

#### Using factories ####
Using the factory pattern, we can move some of the initializing code into another object.
On the cons, factories however won't let us send around a 'sketch' between objects for negotiating.

#### Using flat objects ####
A flat object, or 'use once' factory for CECPEngine could look something like this:
```
class FlatCECPEngine:
    def setGamemodel(model...):
        ...
    def setStrength(strength...):
        ...
    def setName(name...):
        ...
    ...
    def inflate():
        create engine
        start engine
        return engine
```
This pattern may contain the pros of both previous patterns.