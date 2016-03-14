OS X Defaults module for Puppet 4.x
==================

This module manages defaults on OS X.

#Usage

Possible valuse for ``type`` are:

* string
* data
* int
* float
* bool
* data
* array
* array-add
* dict
* dict-add

Example Puppet Code:

	mac_defaults { "set-a4":
          domain => '/Library/Preferences/com.apple.print.PrintingPrefs',
          key => 'DefaultPaperID',
          type => 'string',
          value => "iso-a4",
	}
