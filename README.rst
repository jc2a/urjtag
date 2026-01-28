.. image:: https://travis-ci.org/stappersg/urjtag.png?branch=master
   :target: https://travis-ci.org/stappersg/urjtag
   :alt: Travis CI build status

UrJTAG
======

Software for `JTAG <https://en.wikipedia.org/wiki/JTAG>`

Project homepage is at https://urjtag.sourceforge.io/

Mailinglist is the primary communication channel

This Fork
---------

The 'till-s' branch on this for of urjtag adds a few features to the python bindings but it otherwise
identical to the upstream master:

- Set bsdl path from python. Allows using/finding bsdl files w/o having to update urjtag's database.
- Added `set_signal` and `get_signal` chain methods (analogous to the CLI's `set signal`, `get signal` commands)
- Added `signal_list` chain method to list available signals

These additions allow us to use symbolic references to pins as they are defined in BSDL files.
