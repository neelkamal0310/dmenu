# dmenu - dynamic menu
dmenu is an efficient dynamic menu for X.


## Requirements
In order to build dmenu you need the Xlib header files.


## Installation
Edit config.mk to match your local setup (dmenu is installed into
the `/usr/local` namespace by default).

Afterwards enter the following command to build and install dmenu
(if necessary as root):

`make clean install`

## Applied Patches
* [border](https://tools.suckless.org/dmenu/patches/border/) - Adds a border
  around dmenu. Default width=3. Use `-bw` option to override.
* [center](https://tools.suckless.org/dmenu/patches/center/) - Shows dmenu at
  the center of the screen. Use `-c` switch.
* [grid](https://tools.suckless.org/dmenu/patches/grid/) - Adds an option to
  add columns. Usage: `dmenu -l 5 -g 2` - makes a 5x2 grid
* [nosort](https://tools.suckless.org/dmenu/patches/no-sort/) - Disables
  sorting by name after search. Instead sorts by frequency of use. Enabled by
  -S switch.

## Running dmenu
See the man page for details.
