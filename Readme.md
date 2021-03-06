Introduction
======================

[NBA League Pass](http://www.nba.com/leaguepass/) is an online service offering streaming video of NBA games.

This [XBMC](http://xbmc.org/) plugin features: 

* Archive and condensed games for the NBA 2012 and 2013 seasons
* Live game support
* Fanart from feeds, and thumbnails

The first version of this plugin was written by [robla](http://forum.xbmc.org/showthread.php?tid=124716). Petros Tsampoukas then modified it to work with the 2012 and 2013 NBA seasons, and added images. It requires login.


Installation
=======================

### Requirements

As of 24 March 2014, all games require XBMC Gotham (beta2 or earlier). The archive and condensed games used to work in Frodo but the streams switched to using encryption with HLS, which does not work with Frodo due to faulty cookie support.

See here for a list of nightly builds for your system:

http://wiki.xbmc.org/index.php?title=development_builds#Nightly_build

### Using a zip file

First download the latest version from the [download page](https://bitbucket.org/maxgalbu/plugin.video.nba/downloads#available-downloads). Then install the addon from a zip file in xbmc ([instructions](http://wiki.xbmc.org/index.php?title=Add-on_manager#How_to_install_from_a_ZIP_file)).

### Using mercurial

    cd ~/.xbmc/addons
    hg clone ssh://hg@bitbucket.org/maxgalbu/plugin.video.nba

Changes
=======================

### Changelog:

See changelog.txt

### Potential new features:

* Better thumbnails: display both teams logos. If you are interested to help, let me know!
* Playoff mode: hide the next game of a playoff series
* Filter for favourite team: only show games from your three favourite teams

### Changelog of robla's version:

    0.1.6- bugfix for missing 2012 finals games
    0.1.1- bugfix for missing 2012 finals games
    0.1.0- added listing for complete 2011/2012 season
    0.0.9- fix for new domain watch.nba.com
    0.0.8- fix for playoff game recaps
    0.0.7- fix for archived playoff games
    0.0.6- fix for strange schedule js response
    0.0.5- apply quality settings for highlights, high = 720p
    0.0.4- added highlights and scores
    0.0.3- video idx check
    0.0.2- initial release
    0.0.1- initial test version

### Producing a new zip version

    zip -r plugin.video.nba.v0_6_6.zip -x\*/.hg/\* -x\*/.hgignore -x\*/docs/\* -x\*/*.pyc -x\*/*.pyo plugin.video.nba/
