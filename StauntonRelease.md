# Final Announcement #

We have had a lot of last minute fixes since the release candidate. A few of them for bugs that have been around a long time.
In particular there has been a lot of stabilization of CECP and UCI, so they should now work with an even wider set of engines. You can even run windows engines through wine.

Another important addition to our project is our new website at pychess.org. The website has a good introduction to the client and the community, and in the future it will hopefully be filled with chess related functionality. Sharing your games online could be a great such future.

The main new features of the release are still:
  * Support for chess variants, PyChess now allows you to play Fischer Random with your majors huffled, to play Losers chess with being mated as your goal, or simply playing odds chess as an additional way of giving a player a handicap.
  * On-line play which has been enhanced with chat support. Besides chatting with your opponent, the FICS community has several channels, in which you can discuss chess and varies of other topics.
  * The FICS support has also been improved with built-in Timeseal support. This helps to terminate lag, and is especially helpful in very fast games, like bullet chess.
  * If you prefer to play off-line, PyChess now lets you choose from eight different play-strengths. The built in PyChess engine has as well been extended 'in both extremes' now making many more human like mistakes in the easy mode, and playing at more than double strength in the hard mode, utilizing end game tables.
  * UI-wise, PyChess takes use of a new pure-python docking widget, which lets you rearrange the sidepanels by wish.

I would really like to thank everyone who have helped to move Staunton forward to a release, and I hope our next release - PyChess Anderssen 1.0 - will be out on a slightly shorter cycle.

Please help spread the news of the release to users around the world,
And if you notice that the translation for your language isn't fully updated, head to Rosetta now, and we'll fix it in the 0.10.1 release.

Happy playing,
Thomas Dybdahl Ahle



# Changelog since RC1 #

2011-03-15  leogregianin
  * quick game starts with random color
  * update pt\_BR

2011-03-14  gbtami
  * Fexed draw tests

2011-03-13  Justin Blanchard

  * Make repetitionCount smarter; make the engine treat all repetitions as draws.
  * Fix rep. count in EPD saver. (It's still disabled.) Reps needn't be consecutive.
  * strateval: Only report a pin if it's new.
  * Get EGTBs to work again in PyChess engine.
  * Update constants in egtb\_k4it; don't die from parse errors. Fixes [issue 653](https://code.google.com/p/pychess/issues/detail?id=653).
  * Add EGTB results to bookPanel (1st try)

2011-03-11  gbtami

  * Minor grammar fix in hungarian translation

2011-03-09  Justin Blanchard

  * Don't re-send CECP engines the last move after a setBoard().
  * Fix comment panel promotion error - [Issue 643](https://code.google.com/p/pychess/issues/detail?id=643).
  * Patch on depricated size warnings.
  * Applied bad ponder moves (UCI) from [Issue 648](https://code.google.com/p/pychess/issues/detail?id=648)

2011-03-11  lobais

  * Worked around gtk closure bug
  * Another translatable string
  * Fixed [Issue 638](https://code.google.com/p/pychess/issues/detail?id=638) on multiple monitors.
  * Fix ExpatError/ParseError name change
  * Patch by Uncombed fixing [Issue 651](https://code.google.com/p/pychess/issues/detail?id=651) on loading pgn files to engines.
  * Small fix for [Issue 650](https://code.google.com/p/pychess/issues/detail?id=650)
  * Cleaned up blunders.py output.
  * Removed unused chessFiles references.
  * Working on getting the blunders.py script working again.
  * Add playerUndoMoves and spectatorUndoMoves to Players.py super class.
  * repr may never return Null
  * Patch 647
  * Support specifying engines by path.

2011-03-03  Matthew Gatto

  * Added 'accepted/rejected feature-name' to CECPEngine implementation ([issue 610](https://code.google.com/p/pychess/issues/detail?id=610))
  * Fixed unsupported engines disappearing from engines.xml when their md5sum changes ([issue 616](https://code.google.com/p/pychess/issues/detail?id=616))

2011-01-20  leogregianin

  * correct name of the piece promoted
  * clean name
  * sync with launchpad
  * create website button in about dialog
  * improved button layout
  * update pt\_BR

2011-01-10  gbtami

  * CECP engine fix when san=0 for promotion
  * Fixed [issue #634](https://code.google.com/p/pychess/issues/detail?id=#634)
  * Removed pysqlite import, pychess requires Python >= 2.5 for sime time past

2010-11-11  Matthew Gatto

  * Fixed Odds variants being in the FICS edit-seek dialog and the subsequent KeyError when the user tried to send such a seek
  * Fixed another VERSION import error
  * Fixed VERSION import error
  * Misc typo fixes
  * Removed gettext from setup.py

2010-10-30  thomas

  * Changed == None and != None to is None and is not None, to comply with pep8.
  * Fixed future warning on "not engine"
  * Added logos to devsvg

2010-10-29  gbtami

  * Fix testing if we are installed on system or not
  * Better method for testing if we are installed on the system
  * No need to store the generated PKG-INFO file under version control

2010-10-26  Igor2x

  * Removed extraTranslators hack from [issue 583](https://code.google.com/p/pychess/issues/detail?id=583)

2010-10-26  gbtami

  * Fixed [issue 564](https://code.google.com/p/pychess/issues/detail?id=564) (The very first time Tip of the day text appears selected)
  * Save translators order
  * Distribute ARTISTS and DOCUMENTERS files too
  * Read About dialog data from ARTISTS, AUTHORS, DOCUMENTERS and TRANSLATORS files

2010-10-25  Igor2x

  * Refreshing TRANSLATORS file