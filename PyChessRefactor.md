#PyChess needs a refactor, these are ideas how

# Introduction #

The current structure of PyChess have to major problems:
# It is hard to add new UI modules
# Threads are everywhere

The first problem is a thread to the consistent UI, that is a trademark of PyChess. It is most easily seen at the Fics lounge and chat, which both opens new windows in a way, that makes it hard to say closing which windows will terminate the app.
The problem also makes it hard to get a good grip at plug-ins.

The second problem has been around since the start of PyChess, and has grown more problematic with each release. About 90% of all PyChess crashers (which often are also system crashes) are due to this.

# The solution #

PyChess needs to be refactored into a more modular structure. A structure that makes it clear where to add UI modules and where to lock threads.

# Gedit and Pidgin plug-in structures #

![http://pychess.googlecode.com/svn/wiki/Plug-InExample.png](http://pychess.googlecode.com/svn/wiki/Plug-InExample.png)
![http://pychess.googlecode.com/svn/wiki/pidgin-arch.png](http://pychess.googlecode.com/svn/wiki/pidgin-arch.png)

# Proposed structure #

![http://pychess.googlecode.com/svn/wiki/Diagram1.png](http://pychess.googlecode.com/svn/wiki/Diagram1.png)