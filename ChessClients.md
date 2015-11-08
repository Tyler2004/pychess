# Introduction #
A description of the different chessclients for the linux desktop. Boards are taken in, depending on whether they are inspiring.

  * [CSBoard](ChessClients#CSBoard.md)
  * [glChess](ChessClients#glChess.md)
  * [Chessmonk](ChessClients#Chessmonk.md)
  * [eboard](ChessClients#eboard.md)
  * [Jin](ChessClients#Jin.md)
  * [Jose](ChessClients#Jose.md)
  * [Scid](ChessClients#Scid.md)
  * [Scid vs. PC](ChessClients#Scid_vs._PC.md)
  * [Scidb](ChessClients#Scidb.md)
  * [ChessX](ChessClients#ChessX.md)
  * [New Generation Board](ChessClients#New_Generation_Board.md)
  * [Mono Chess](ChessClients#Mono_Chess.md)
  * [Tagua](ChessClients#Tagua.md)
  * [Kaya](ChessClients#Kaya.md)
  * [Ceibal](ChessClients#Ceibal.md)
  * [flashCHESS\_III](ChessClients#flashCHESS_III.md)
  * [Raptor](ChessClients#Raptor.md)
  * [Cute Chess](ChessClients#Cute_Chess.md)
  * [Lucas Chess](ChessClients#Lucas_Chess.md)
  * [Knights](ChessClients#Knights.md)
  * [Lantern Chess](ChessClients#Lantern_Chess.md)

[Further reading](ChessClients#Further_reading.md)


---


# CSBoard #
CSBoard is a small GUI for gnuchess. It is written in C# and uses gtk-sharp and mono.

  * Supports CECP engines
  * Supports ICS over FICS with nice gui
  * Support for PGN files including comments
  * Print games, or export them as a PostScript file
  * Has a chessdatabase, to store rated and tagged games
  * Official webpage: http://csboard.berlios.de/


---


# glChess #
glChess is a 2D/3D chess game for Unix.

  * glChess is part of the Gnome Games.
  * Written in Python and PyGTK.
  * Games can be played between a combination of human and chess engines.
  * Network games still not implementation.
  * glChess support 3D using OpenGL.
  * Official webpage: http://glchess.sf.net


---


# Chessmonk #
Chessmonk is a completely functional PGN viewer with an attractive interface.

  * Scalable board with SVG piece graphics.
  * move animation, a game list and a detailed display of the notation.
  * Internet chess not implementation.
  * Written in Python, PyGTK.
  * Official webpage: http://code.google.com/p/chessmonk/


---


# eboard #
eboard is a chess interface for Unix-like systems (GNU/Linux, FreeBSD, Solaris, etc.) based on the GTK+.

  * Support internet chess ICS and FICS.
  * Support chess engines.
  * Reads and writes chess games in PGN format.
  * Configurable interface (board and pieces).
  * Support DGT electronic chess board.
  * Support scripts (Perl).
  * Written in C++.
  * Official webpage: http://www.bergo.eng.br/eboard


---


# Jin #
Jin is an open source, cross platform, graphical client (aka interface) for chess servers.

  * Jin is a standard chess client for FICS http://freechess.org/Login/jin/applet.php
  * Supports FICS and ICC.
  * Written in Java.
  * Run installed in your machine or with Java applet.
  * Official webpage: http://jinchess.com/


---


# Jose #
Jose is a graphical Chess tool.
You can store chess games in a database (backed by MySQL).
You can view games and edit variations and comments.
You can play against a "plugged-in" chess engine and use it for analysis.

  * graphical frontend to MySQL database
  * read and write PGN (Portable Game Notations) files
  * 2D and 3D view
  * edit games, insert comments, variations
  * plug-in chess engine for play and analysis; supports both XBoard and UCI protocol.
  * Play Fischer Random Chess / Chess 960, or Shuffle Chess
  * Opening Books
  * ECO opening classification
  * Position Search
  * Create HTML and PDF files.
  * Web Servlet interface
  * Written in Java.
  * Official webpage: http://jose-chess.sourceforge.net


---


# Scid #
Scid ("Shane's Chess Information Database") a chess database application for Windows and Linux operating systems.

  * View graphical trends and produce printable reports.
  * Support chess engines.
  * Scid support FICS internet chess.
  * Written in C++ and Tcl.
  * Official website: http://scid.sourceforge.net


---


# Scid vs. PC #
Scid vs. PC is a usability and bug-fix fork of Scid.
  * Official website: http://scidvspc.sourceforge.net


---


# Scidb #
Scidb is inspired by Scid, but it is a completely new development.
  * Official website: http://scidb.sourceforge.net


---


# ChessX #
ChessX is a chess database. With ChessX you can operate on your collection of chess games in many ways: browse, edit, add, organize, analyze, etc.

  * Multi-platform. Supports Linux, Microsoft Windows and Mac OS
  * Load and save PGN files
  * Work with multiple databases simultaneously
  * Browse games
  * Navigate through game, including variations
  * Copy/Paste FEN
  * Enter moves, setup board position
  * Basic header search (click on columns in GameList header)
  * Player database with statistics
  * Chess engine support
  * Written in C++ (Qt4)
  * Official website: http://chessx.sourceforge.net


---


# New Generation Board #
Next generation chess application for GTK. With freechess.org support, unicode, SVG scalable graphics, sounds and more!

  * Plays chess on FICS or against a computer
  * Contains many board themes
  * Lets you browse and analyse stored games
  * Comes with a python implementation of timeseal for fics
  * Official website: http://ngboard.sourceforge.net/news.php


---


# Mono Chess #
MonoChess is an interface for play against xboard chess engines and in a future connect to ics servers. It has an excellent sense of aesthetics, but is currently quite simple.

  * CECP Engine support
  * ScoreSheet
  * Opening book? (Seams to be implemented, but doesn't work as of this writing)
  * Official website: http://code.google.com/p/monochess/w/list


---


# Tagua #
Tagua (previously known as KBoard) is a generic board game suite for KDE, including games like Chess, Shogi, Xiangqi and variants. Tagua is based on a powerful plugin system that allows many games to share the same graphical framework, game history handling, interoperability with AI engines and connectivity to network servers.

  * Playing against the computer (CECP)
  * Local editing of games
  * FICS / ICC compatible server support using a detachable console
  * Tons of variants are supported. E.g. Shogi, Atomic, Monster Chess
  * Advanced graphics and animations
  * Official website: http://tagua-project.org/


---


# Kaya #
Kaya is a board game suite, containing games such as Chess and Shogi, and built upon a powerful plugin system which makes it easily extensible with new games, themes and behaviour.

  * Written in Ruby (Qt4)
  * Supported games: Chess, Minichess, Shogi, Minishogi, Crazyhouse.
  * Game history sidebar.
  * Customizable interface.
  * FICS support: play, examine and observe games, interact using a text console.
  * Load, edit and save chess and shogi games.
  * XBoard-compatible chess engine support.
  * GNU Shogi engine support.
  * Official website: http://paolocapriotti.com/kaya/


---


# Ceibal #
Ceibal-chess is about creating a Chess activity for the Sugar environment (in particular for the OLPC XO laptops) to teach kids the basic rules of the game and allow them to play with one another and vs. the CPU.

  * GPL v2 license
  * Designed from the ground up to work on the XO.
  * Distributed as an Activity Bundle (.xo)
  * Completely developed in Python + PyGame.
  * Integration with GNU Chess.
  * Player vs Player mode
  * Valid movements highlighting.
  * Enemy movements highlighting.
  * Portable: known to work on various Linux distros and Mac OS X.
  * Easy to learn and use, without complex menus or options.
  * Official project site: http://code.google.com/p/ceibal-chess


---


# flashCHESS III #
Flashchess is a free (to play) online chess game. It is written in flash, and contains some nice quick to play features.

  * 3D Board
  * Easy to beat opponent
  * Official project site: http://www.flashchess3.com/


---


# Raptor #
Raptor is a cross platform chess interface and pgn viewer for the free internet chess server: FICS.

  * Written in Java
  * Features: http://code.google.com/p/raptor-chess-interface/wiki/Features
  * Official project site: http://code.google.com/p/raptor-chess-interface/


---


# Cute Chess #
Cute Chess is a set of cross-platform tools for working with chess engines. It consists of:
  * cutechess—a graphical user interface.
  * cutechess-cli—a command-line interface for automating chess engine matches.
  * libcutechess—a library providing an interface for working with chess engines.
  * Written in C++ and Qt
  * Official project site: http://ajonsson.kapsi.fi/cutechess.html


---


# Lucas Chess #
To play against the computer and to train chess. One important feature is to play chess with increasing levels of difficulty and with a limited number of hints that are given by a chess tutor. Also included are thousands of training positions such as different types of endgames, tactical combinations and chess problems (mate in 2,3,4 and more).

  * Written in Python (Qt4)
  * Official project site: http://code.google.com/p/lucaschess/


---


# Knights #
Knights is the chess interface for KDE SC 4. It features play against opponents on the Free Internet Chess Server, a friend on the same computer, or a computer chess engine.

  * Official project site: http://noughmad.com/knights/


---


# Lantern Chess #
ICC Client for Mac Windows and Linux

  * GPL License
  * Written in Java
  * Official project site: http://www.lanternchess.com/


---


# Further reading #
The above list was inspired by [a similar one](http://bobthegnome.blogspot.com/2006/12/summary-of-current-open-source-chess.html) made by Robert Ancell in the end of 2006.

The German ubuntuusers wiki has done a feature to feature comparison of all chess interfaces in ubuntu. It is good reading, even though it compares only PyChess Greco. http://wiki.ubuntuusers.de/Schachsoftware