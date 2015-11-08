## New Release Checklist ##
When a beta has been declared stable, we'll have to do the following:
  * Update const.py with new version
  * Check out a fresh trunk
  * Create rpm using guide in INSTALL
  * Notice deb maintainer of the release
  * Deprecate old rpm's, deb's and tgz's from google code downloads and add new files
  * Add notice on the pychess.googlepages.com frontpage
  * Edit features / TODO list in the FAQ section.
  * Update gnomefiles, freshmeat, pypi, gtk-apps and happypengiun pages
  * Spread the message to gnomedesktop.org, linuxgames.com, python-announce-list@python.org

## First beta release ##
When a branch has become stable enough to go beta, we'll have to do the following:
  * Create translation template and notice translators
  * Create rpm using guide in INSTALL
  * Notice deb maintainer of the release
  * Deprecate old rpm's, deb's and tgz's from google code downloads and add new files
  * Update gnomefiles page
  * Add notice on the pychess.googlepages.com frontpage

## Create translation template ##
  * Run create\_template.po.sh script to get a po file of all pychess string
  * Run the following command to get the comments from the old template merged into the new one.
```
msgmerge lang/template.po newtemplate.po -o lib/template.po
```
  * Add template to rosetta

## New translation added ##
  * Add translation to hg
  * Add translator to TRANSLATORS

## New developer added ##
  * Add to google code
  * Add to AUTHORS