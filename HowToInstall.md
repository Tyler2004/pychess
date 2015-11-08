# Introduction #

Different Linux distributions require different procedures for the installation.

## Run only (from source without installing) ##
Download the latest release (.tar.gz version) from <a href='http://pychess.org/download/'><a href='http://pychess.org/download/'>http://pychess.org/download/</a></a><br>
After extracting the tar.gz, run the following command in the extracted directory<br>
$ ./pychess<br>
<br>
<h2>Debian / Ubuntu</h2>
$ apt-get install pychess<br>
<br>
<h2>Red Hat / Fedora / CentOS</h2>
To install the latest release (<b>recommended method</b>), first check your python version:<br>
$ python --version<br>
Python 2.7.5<br>
Then download the latest release (py27.noarch.rpm version in our case) from <a href='http://pychess.org/download/'><a href='http://pychess.org/download/'>http://pychess.org/download/</a></a> and:<br>
$ yum install ~/Downloads/pychess-LATEST-VERSION.py27.noarch.rpm<br>
<br>
Or, to install the distribution supplied version:<br>
$ yum install pychess<br>
<br>
<h2>Arch Linux</h2>
$ pacman -S pychess<br>
<br>
<h2>SuSE / openSUSE</h2>
not yet<br>
<br>
<h2>Gentoo</h2>
$ emerge pychess<br>
<br>
<h2>Mandriva</h2>
not yet<br>
<br>
<h2>Slackware</h2>
not yet