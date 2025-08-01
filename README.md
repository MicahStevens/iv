iv -- Image Viewer
=========================

A simple image viewer that can recursively display images from directories in a
grid. Click on any image to display it full size. Auto-reloads images if
they are changed on disk.

Supports all image formats used on the web including animated GIFs and SVG.

Uses a browser engine (chromium) to do the rendering, so its format support
will always be current.

**Enhanced Features:**
- Wallpaper setting integration with `swww` for Hyprland desktop
- Quick exit shortcuts for improved workflow

Original author: [Kovid Goyal](https://github.com/kovidgoyal/iv)  
Enhanced by: [Micah Stevens](https://github.com/MicahStevens)

Dependencies
==============

* python >= 3.5
* PyQt >= 5.7
* rapydscript-ng >= 0.7.9

Installation
==============

Simply clone this repository and run it using

```
python3 /path/to/cloned/repository /path/to/image/directory
```

Controls
===========

`iv` is largely keyboard controlled. The keyboard shortcuts in the two views are:

Grid View
-------------

* `c` - Toggle the captions
* `+` - Increase thumbnail size
* `-` - Decrease thumbnail size
* `0` - Reset thumbnail size to default
* `r`, `F5` - Reload all thumbnails
* `j` - Scroll down
* `k` - Scroll up
* `w` - Set hovered image as wallpaper (requires `swww`)
* `x` - Exit application
* `Esc` - Exit application

Single Image View
-------------------

* `c` - Toggle the information display
* `+` - Zoom in
* `-` - Zoom out
* `0` - Reset zoom to no zoom
* `r`, `F5` - Reload image
* `Esc` - Go back to the grid view
* `Space`, `Right`, `Down`, `Pagedown`, `j` - Show next image
* `Backspace`, `Left`, `Up`, `Pageup`, `k` - Show previous image
* `w` - Set current image as wallpaper (requires `swww`)
* `x` - Exit application
* Right-click - Show context menu with wallpaper option
