# Introduction #

PyChess has a number of features not well known to many.
They aren't built into the PyChess client, like most other features, but rather live a simple life in the `utilities/` folder, until it is decided what to do with them.

As simple scripts, they serve as a great way to get started on hacking PyChess, but they are also useful in the features they have. On this page we'll describe some of them.

## Blunder checking ##

After you've played a long game on the web, or versus an engine, you may wonder how you could improve your game, so it's tip top for the next one.
In chess, a common way to do this, is to analyse your game for bad moves, or blunders.

The `utilities/blunders.py` will help you on this task in a number of ways:
  * It will tell you, if your opponent made a mistake, that you didn't take advantage of.
  * It will tell you, if you made a mistake, that your opponent didn't take advantage of.
  * It will tell you what you could have done instead, to avoid the bad position.

Below is an example of a short game analysed by the PyChess engine. The user remembered to save the game as a pgn file after he or she finished.

```
[user@localhost utilities]$ PYTHONPATH=../lib/ python blunders.py ~/myShortGame.pgn 
Selected file ~/myShortGame.pgn

The file contains the following games:
[0] User vs. Guest

Autoselecting game 0.

PyChess found the following analyzers on your system:
[0] PyChess 0.10rc1
[1] GNU Chess 5.07
[2] Dee Rybka

What engine should be your analyzer? [n] 0

Enter how many seconds we should use for each move [n]: 10

PyChess 0.10rc1 will now analyze the game between Unknown and Unknown with 10 seconds per move.

.......
Considering 5 Ng8  ....
Considering 4 Ng1  .....
White blunder -119
Should have done: Nc3, e6, Ng5, Qe7, Nxh7, Nxh7

Considering 4 Nf6  .....
Considering 3 Nf3  .....
Considering 3 Ng8  .....
Considering 2 Ng1  .....
Considering 2 Nf6  .....
Considering 1 Nf3  ..... Finish
```

## The Arena ##

Have you ever wondered which of your installed engines is stronger? Perhaps you have made small tournaments in the interface, noting who beat who. That isn't very efficient though. A much better choice is to use th `utilities/arena.py` script, as shown below:

[user@localhost utilities]$ PYTHONPATH=../lib/ python arena.py 
Discovering uci engines
Your installed engines are:
[PyC] PyChess 0.10rc1
[GNU] GNU Chess 5.07
[Dee] Dee Rybka
The total amount of fights will be 6

Please enter the clock minutes for each game [n]: 1
The games will last up to 12 minutes.
You will be informed of the progress as the games finish.

Starting the game between PyChess 0.10rc1 and GNU Chess 5.07
The game between PyChess 0.10rc1 and GNU Chess 5.07 ended 0-1
The current scores are:
W\B PyC GNU Dee
PyC  #  0-1  . 
GNU  .   #   . 
Dee  .   .   # 

Starting the game between GNU Chess 5.07 and PyChess 0.10rc1
The game between GNU Chess 5.07 and PyChess 0.10rc1 ended 1-0
The current scores are:
W\B PyC GNU Dee
PyC  #  0-1  . 
GNU 1-0  #   . 
Dee  .   .   # 

Starting the game between PyChess 0.10rc1 and Dee Rybka
The game between PyChess 0.10rc1 and Dee Rybka ended 0-1
The current scores are:
W\B PyC GNU Dee
PyC  #  0-1 0-1
GNU 1-0  #   . 
Dee  .   .   # 

Starting the game between GNU Chess 5.07 and Dee Rybka
The game between GNU Chess 5.07 and Dee Rybka ended 1-0
The current scores are:
W\B PyC GNU Dee
PyC  #  0-1 0-1
GNU 1-0  #  1-0
Dee  .   .   # 

Starting the game between Dee Rybka and GNU Chess 5.07
The game between Dee Rybka and GNU Chess 5.07 ended 0-1
The current scores are:
W\B PyC GNU Dee
PyC  #  0-1 0-1
GNU 1-0  #  1-0
Dee  .  0-1  # 

Starting the game between Dee Rybka and PyChess 0.10rc1
The game between Dee Rybka and PyChess 0.10rc1 ended 1-0
The current scores are:
W\B PyC GNU Dee
PyC  #  0-1 0-1
GNU 1-0  #  1-0
Dee 1-0 0-1  # 

All games have now been played. Here are the final scores:
GNU Chess 5.07 : 4 
Dee Rybka : 2 
PyChess 0.10rc1 : 0 ```