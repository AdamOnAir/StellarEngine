# Stellar Engine - A game engine for Airlib.

Stellar Engine is an open source, cross-platform 2D graphics engine for [Airlib](https://adamonair.neocities.org/airlib).

## Features
* Written in C
* MPL License: free for any project, including commercial ones, allows console development
* Cross platform: available builds for Windows (32/64) and Linux PC(32/64).
* High performance: OpenGL based, runs fastly as Airlib uses native libraries(WinAPI/GLX)
* Streamlined, easy to learn API that requires very little lines of code
* Built-in Airlib-based windowing for quick tests
* Loads assets from open standard file formats
* Create or modify graphic assets procedurally at run time
* True raster effects: modify render parameters between scanlines
* Background layer scaling and rotation
* Sprite scaling
* Several blending modes for layers and sprites
* Pixel accurate sprite vs sprite and sprite vs layer collision detection
* Special effects: per-column offset, mosaic, per-pixel displacement, CRT emulation...
* Supports packaged assets with optional AES-128 encryption

# Getting binaries

## Download from itch.io
The recommended way to get prebuilt binaries ready to install, run and test samples is grabbing them from official [itch.io download](https://megamarc.itch.io/Stellar Engine). Just download the package for your platform, they contain required dependencies to run.

## Build from source
You can also build the library from source. Stellar Engine requires `SDL2` and `libpng` to build, you must provide these libraries yourself depending on your target platform.

### Windows

You must provide development libraries:
* libpng: http://gnuwin32.sourceforge.net/packages/libpng.htm

Put the following files inside the `src` directory:
Path | Files
-----|---------------------------------------
`src\libpng`             | libpng headers
`src\libpng\$(Platform)` | libpng.lib import library

### GNU/Linux
Just install standard packages `libpng-devel` and `SDL2-devel`.
  
Once installed, open a console window in the C samples folder and type the suitable command depending on your platform:

## Windows
```
> mingw32-make
```

## GNU/Linux
```
> make
```
