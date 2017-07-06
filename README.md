# Quarter Tiling Script for KWin

## Features
- Tiles windows
- Maintains the tiled layout when windows are interacted with
- Automatically creates and switches virtual desktops
- **Shortcut to exclude windows (Meta+F by default)**
- ** To bind shortcuts go to settings -> shortcuts -> global shortcuts -> kwin and search for "Quarter" to find all the script specific shortcuts!**


## Screenshots

#### Movement keys:
![Keybindings](http://imgur.com/W3HzO5A.gif)

#### Screenshot with three windows:
![Screenshot](https://u.teknik.io/IZz6t.png)

[Video demonstration (a gfycat link)](https://gfycat.com/TintedRepentantKawala)


## Installation
- Move or clone to ~/.local/share/kwin/scripts and enable the script via KWin Scripts

## Help
- In case Meta+F is not working, go to settings -> shortcuts -> global shortcuts -> kwin and search for "Float", bind a shortcut for the action "Float On/Off"
- In case of trouble, restart the script by disabling it and enabling it again via KWin Scripts
- To adjust gapsize, edit /contents/code/main.js, find var gap and change the integer
- To disable borders, edit /contents/code/main.js, find var noBorders and change the boolean
- To add/remove programs from the blacklist edit /contents/code/main.js and add/remove entries from ignoredClients
- If above does not work, try adding a recognizable and unique part of the window caption to ignoredCaptions

## Note
- If you remove a virtual desktop, all of the tiled clients on the desktop will also be closed
- Virtual desktops are not automatically removed because doing so via script crashes plasma (I suspect it's a plasma bug)
- Some programs, like Spotify can not be recognized or automatically excluded. If you use such programs, use Meta+F to disable them to avoid problems.

## Upcoming features
- Configuration interface
- Window resizing
- Support for chosen programs to always occupy at least half of the screen
