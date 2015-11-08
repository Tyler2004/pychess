# Introduction #

This is very much unfinished notes.

PyChess should be the chess client for players levels between "new" and "advanced hobbyist". It should thus be easy while powerful, encouraging while simple, and fun.

To reach the two end segments, we need to have more features for analysis as well as a more welcomming face for new players. Most of all we need a better overview on the features we have and a

# The four tabs UI #

A chess client is among other things a working environment. Another working environment with multiple "workspaces" is an IDE. Eclipse has chosen a system of "perspectives" which are workspaces furnished by the users with "views".

# Mockups (svg) #
You need to open these in an editor, like inkscape, to get the full image, as a lot of stuff is outside the canvas.
  * [Welcome screen](https://www.dropbox.com/s/7fgaufzpeloh84l/welcome.svg)
  * [Backstage screen](https://www.dropbox.com/s/547xpzf2naen0ov/backstage.svg)
  * [Playing screen](https://www.dropbox.com/s/a8k39d9hy9klpv6/playing.svg)
(Notice: Open those in Inkscape, as they are not quite standard svg)

## Other dialogs ##

### The engine lounge ###

Will let you manage engines.
It is not a real 'workspace', so it doesn't get its own tab, but rather a dialog from the Tool menu.
  * Lets you add/remove
  * Lets you create personalities / configure
  * Lets you do engine tournaments - in order to rate engines.

### The fics lounge ###
This could be sweet to avoid, by integrating the parts around in the ui.

# Tabbed view #
Two workspaces could benefit from a tabbed view: Playing and Analyzing.
However normally you only play a single game at a time, so tabs would only be for observing.
Also, as the 'tabs' are for observing, minitures would be more fitting, maybe with a viewmode switch between 'side by side' and 'one big + some small'.

The trouble is (or might be), that giving each workspace a different tabbed mode, is not very consistent.

# In the back #
  * For easier overview of the code, we need a more modular style. Likely with extension support.
  * The threads needs a strategy.

# Ideas not currently fitting in #
  * Use PyChess to organize tournaments. Some people would like pychess to create tournament tables for print. Others would like to participate in a tournament with engines. Finally fics has some support for tournaments.
  * Recommended observes. - These GMs are playing today. Actually just a way to start observes and get fics news.