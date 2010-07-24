# Uncrustify Automator Services for Xcode 4 developer preview #

- Version: 0.1
- Date: Saturday, 24 July 2010
- Author: Tony Arnold, tony@thecocoabots.com
- Requirements: Xcode 4 developer preview 2, Mac OS X 10.6.4

## What's it do? ##

These automator scripts allow you quickly reformat your code using the brilliant `uncrustify` command-line utility ([http://uncrustify.sf.net/](http://uncrustify.sf.net/)). The scripts assume that you have `uncrustify` installed in `/usr/local/bin` - I'd suggest using something like [Homebrew](http://mxcl.github.com/homebrew/) to do this.

A sample Objective-C uncrustify configuration file is available at [http://gist.github.com/261662/](http://gist.github.com/261662/) - just copy or move this file to `~/.uncrustify.cfg` to use it.

## Installation ##

Copy or move the included workflow files into `~/Library/Services/`.

## How do I use it? ##

### A note of caution ###

Uncrustify will write over your source files with it's changes without asking you if you choose to operate on an entire document. If you want to see what changes will be made without writing over your files, select all the code in your current Objective-C file and use the "*Uncrustify Selected Text*" service.

### How to ###

1. Open a document (or multiple documents), or select text in an already open document;
2. Go to the **Xcode** menu, then select *Services* and make your choice from the scripts starting with "*Uncrustify...*".

Xcode will ask you if you want to revert to the file on disk - selecting "*Revert*" will show the changes uncrustify has made. 

## Copyright ##

Copyright 2010 Tony Arnold. See LICENSE for details.