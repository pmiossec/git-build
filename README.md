git-build
=========

Git script to prevent the use of a Continuous Integration Server by running a custom command (e.g. build and test) before pushing to a repository

This script made it easier to run a private build before pushing your modifications in order to compile and run your unit test.

# Install

* Copy all the files (respecting the names) in a folder that is in your path
* If you are under Windows, install [Growl for Windows](http://www.growlforwindows.com/gfw/)

# Use

* For each new git repository you use and only one time, set the command that will be run before pushing

Example using maven :

`git config private-build.command "mvn clean install"`

* call `git build` each time you want to push!
