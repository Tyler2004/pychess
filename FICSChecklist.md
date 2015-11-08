# Introduction #

These are the features which need to be implemented to have a fulle featured FICS client. Support for more chess servers can be added later.

# Checklist #
X is done. % is not.
```
    Game list
          X Show
          X AutUpdate
          X Observe game
                X Sync clock
                X Get prior moves
                X Get initial board (on resumed games)
                X Understand status changes
                      X Draw
                      X Win
                      X ...
                X Understand other actions
                      X Takeback
                      X Switch side
                      X Pause/Unpause
                      X Offer draw
         % Examine game
                % Recognize game type
                % Attach whisper, kibitz chat ui to game
    People list
          X Show
          X Autupdate
          % Follow
          X Show info on players (click: 'start private chat' w/ player selected in Player List tab.
            Will be better when we implement profiles and have rating/strength graphs)
          X Challenge players
    Lists management
          % Friends list (aka notify list)
          % Censor list
          % No-play list
    Seek/Challenges list
          X Show
          X Autupdate
          X Seek Graph
          X Make seeks acceptable
                X Make offers offerable and acceptable (Need to show list of incoming and outgoing offers)
                      X Pause, Unpause
                      X Draw
                      X Abort
                      X Adjourn
                      X Takeback
                      X Switch side
          X Show challenges
                X Make challenges acceptable
                X Make challenges declinable
    Adjourned list
          X Show
          X Autupdate
          X Resign game
          X Offer draw
          X Offer resume
                X Load the board the model
          X Offer abort
    Seeker
          % Make filtering work (I think fics formula feature already does this)
          X Make Seeking work
    Infopanel
          X Game name
          X Get rating info
          X Get online time info
          X Get ping
          X Get email
    Chat
          X Create ChatManager
          X Make interface work
    Console
          X Find out which information to show
          X Make interface work
    Variants
          X Atomic
          % Bughouse
          X Crazyhouse
          X Standard
          X Losers
          X Suicide
          X Wild/fr (fischerandom)
          X Wild/0  (wildcastle)
          X Wild/1  (shuffle wildcastle)
          X Wild/2  (shuffle nocastle)
          X Wild/3  (random)
          X Wild/4  (asymmetric random)
          X Wild/5  (upside down)
          X Wild/8  (pawns pushed)
          X Wild/8a (pawns passed)
```


