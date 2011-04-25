# Uncrustify Automator Services for Xcode 4 #

- Version: 0.4
- Date: Thursday, 14 April 2011
- Author: Tony Arnold, tony@thecocoabots.com
- Requirements: Xcode 4.0 or higher, Mac OS X 10.6 or higher

## What's it do? ##

These automator scripts allow you quickly reformat your code using the brilliant `uncrustify` command-line utility ([http://uncrustify.sf.net/](http://uncrustify.sf.net/)).

A sample Objective-C uncrustify configuration file is available at [http://gist.github.com/261662/](http://gist.github.com/261662/) - just copy or move this file to `~/.uncrustify.cfg` to use it.

## Installation ##

I will assume you have a basic understanding of installing software using a package manager like [Homebrew][hb].

 1. Install **uncrustify**. I use [Homebrew][hb] to do this — `brew install uncrustify` — but you could just as easily do it by hand, or ;
 2. Make sure that **uncrustify** is in your `$PATH` — you can verify this by opening a new terminal window and typing `which uncrustify` — if the full path to your copy of **uncrustify** is printed, you're set;
 3. Copy or move the included workflow files into `~/Library/Services/`.

## How do I use it? ##

### A word of caution ###

Uncrustify will write over your source files with it's changes without asking you if you choose to operate on an entire document. If you want to see what changes will be made without writing over your files, select all the code in your current Objective-C file and use the "*Uncrustify Selected Source Code*" service.

### How to ###

1. Open a document (or multiple documents), or select text in an already open document;
2. Go to the **Xcode** menu, then select *Services* and make your choice from the scripts starting with "*Uncrustify...*".

Xcode will ask you if you want to revert to the file on disk - selecting "*Revert*" will show the changes `uncrustify` has made. 

## Copyright ##

Copyright 2010—2011 Tony Arnold. See LICENSE for details.


 [hb]: http://mxcl.github.com/homebrew/