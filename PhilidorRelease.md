# 0.8.1 Release #
While the work on Stauton is fastly progressing, a few bugs has been reported on the Philidor release. These should now be fixed.
  * Made PyChess start a game correctly when choosing Black.
  * Fixed window resize problems on start-up
  * Fixed icon lookup error on some systems
  * Added port 5000 as alternative for FICS
  * Fixed some button size problem with the industrial themes
  * Made PyChess indentify itself on FICS, to support the statistics

# Final Announcement #
PyChess Philidor 0.8 has been released. This happens after nearly a year
coding, and a rewrite of large parts of the codebase for stability and
features. If you haven't already beaten fruit, gnuchess, pychess-engine
and your friend with PyChess, now is time to!

The most prominent new features include:
  * Online chess play on the FICS servers.
  * Ability to undo and pause chess games.
  * Support for UCI engines like Fruit, Glaurung and Shredder.
  * Full list of changes: http://code.google.com/p/pychess/wiki/PhilidorRelease

The development of PyChess Stauton 1.0 has just begun. We strive to make
this the greatest free chess client out there, so if you have opinions,
don't let them go unheard on the mailing list!

If you would like help fix the translation of PyChess in your language,
see http://code.google.com/p/pychess/wiki/RosettaTranslates to get
started.

  * Full list of features: http://pychess.googlepages.com/about
  * Downloads: http://code.google.com/p/pychess/downloads/list
  * Screenshots: http://pychess.googlepages.com/screenshots
  * Mailing list: http://groups.google.com/group/pychess-people



# Final Changelog #

  * Updated translations
  * Fixed combobox width problem
  * Don't set the gstreamer pipeline to playing if the uri is not set
  * Made score panel keyboard navigateable
  * Fixed d'n'd indentifier problem on 64bit systems ([issue 301](https://code.google.com/p/pychess/issues/detail?id=301))
  * Fixed .desktop file ([Issue 299](https://code.google.com/p/pychess/issues/detail?id=299))

# Beta 4 Changelog #

PyChess Philidor 0.8 beta4 has been released! This fixed a lot of problem that people have reported, and includes translations in more than 23 languages.
If no more serious bugs are found, this will be named final, but in order to ensure everything is perfect please check it out and tell us what you think!

As always you can find screenshots at: http://pychess.googlepages.com/screenshots
And you can help translating at: https://translations.launchpad.net/pychess

  * Made new games start more smoothly
  * Made pgn-load errors more informative
  * Added Toga 2 to supported UCI engines
  * Added translations from Rosetta
  * Made PyChess easier to beat on easy levels
  * Made opening files from the commandline, or over http, work better
  * Made PyChess never resign, so that people have the fun of mating

  * Fixed a problem, which made engines unable to undo in loaded games
  * Fixed a problem, which made engines freeze on pause
  * Fixed a problem, which made PyChess try to use nonexecutable engines
  * Made PyChess search more than 0 secs when playing without clock
  * Fixed problem that made analysers corrupt gamedata
  * Fixed a problem, which killed the second started engine in some python versions

  * Fixed an import problem on gtksoureview
  * Fixed an Unicode problem for translations
  * Added missing spaces in FICS news
  * Fixed a FICS problem on adjourned games
  * Fixed a problem, which made file menu items insensitive
  * Fixed a bug, which made NewGameDialog deallocate when closing
  * Fixed ugly output from gstreamer and ChessClock on app closing
  * Made BoardView properly mark last move after loading game
  * Enabled sorting of games on FICS
  * Fixed a problem that made enterGameNotation panel very small
  * Made it possible to load empty files (They will just start a normal game)
  * Made PyChess ignore non-chessfiles drags
  * Fixed PyChess not remembering side panel state
  * Implemented the python 2.6 way to avoid random errors when daemon threads wake up
  * Fixed scorePanel to show initial position
  * Added better debugging
  * Fixed prefix problem in leval's evalKingTrophism for black

# Beta 3 Changelog #

I'm pleased to announce, that a new PyChess Philidor 0.8 beta has been made available.

It was headed as a Christmas release, and it contains the following changes:

  * Fixed a gtk/threading bug in loading files from command line
  * Fixed an IndexError when the count of installed engines shrunk
  * Fixed bugs in -, and improved logging
  * Cleaned up shortcut and accelerator keys

  * Made side panel hide properly in FICS games
  * Fixed typos in rarely touched code
  * Added better distinction between manually and automatically accepted seeks
  * Disabled sound availability test, as it produced false positives

  * Made load preview show the latest, rather than the earliest, position
  * Faster parsing of SAN moves and PGNs
  * Improved engine path handling
  * Made gstreamer optional

As Tamás has found some pretty critical further issues, it might take one or two more beta releases before we can declare it final.

Also, the larger Philidor text-base isn't yet translated to near to number of languages that Greco had, so if you feel like it, head to https://translations.launchpad.net/pychess and make some noise!

However, merry Christmas, or happy holiday season to your all!

# Beta 2 Changelog #
Fics:
  * Autoanswer private chat messages
  * Autodecline adjourn challenges
  * Fixed a racecondition in ServerPlayer
  * The ratingtable should update after game ends
  * Fixed a problem, where a player could bring up two iclounges if pressing the connect button heavily enough
External engines:
  * Fixed cecp undo bug
  * Made sure engines are restested next time PyChess start
Builtin engine:
  * Better time control
  * Minor speedups
  * Fixed bug in quienscent search
  * depth check in transposition table
Interface:
  * Made "Use Sound" checkbutton insensitive when gstreamer sees errors

# Announcement #
After the by far longest PyChess development cycle, version Philidor beta, codenamed 0.8 beta, has been released!

Download from: http://gnomefiles.org/app.php/PyChess

Screenshots: http://pychess.googlepages.com/screenshots

The long development time covers a close to total rewrite, the most throughout testing for a PyChess release yet, and a massive new base of features. Many of which users have been screaming since the first alpha of PyChess.

The new features includes, but are not restricted to:
  * FICS online Internet play.
  * Undo and pause functions.
  * Support for UCI engines like Fruit, Glaurung and Shredder.
  * Ability to turn analysers on/off, and to decide which engines should be used.
  * An "Enter game" in pgn dialog.
  * New fast start greeting screen.
  * A 30x faster built in python engine.
  * Internationalized or figure pieces in notation .
  * Optional sounds.
  * A comments side panel that helps you understand the moves made.
  * Pychess now use Launchpad Rosetta for i18n

It should be noted, however, that even though the FICS implementation is generally very stable, it hasn't yet got support for chatting and console communication. Thus it should be used with some care.

We encourage everyone to try out the release, and report the bugs (if any) you find.

If you'd like to see PyChess translated into your language, you can help us from the web interface at https://translations.launchpad.net/pychess/trunk/+pots/pychess

And remember: "The Game of Chess is not merely an idle amusement; Several very valuable qualities of the mind, useful in the course of human life, are to be acquired and strengthened by it" - Benjamin Franklin, 1779

Thanks,
Pychess team

  * Homepage: http://pychess.googlepages.com
  * Screenshots: http://pychess.googlepages.com/screenshots
  * Project page: http://code.google.com/p/pychess
  * Downloads: http://code.google.com/p/pychess/downloads/list
  * Bug list: http://code.google.com/p/pychess/issues/list
  * Mailing list: http://groups.google.com/group/pychess-people