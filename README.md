# xcompmgr-simple-opacity
An extremely small and fast xorg windows compositor that adds transparency to your desktop environment

This is a fork of [jmanc3's xcompmgr-simple](https://github.com/jmanc3/xcompmgr-simple) whose purpose is to simplify [xorg's xcompgmr](https://gitlab.freedesktop.org/xorg/app/xcompmgr) code base to only implement window transparency using ARGB. That code however removed the support for global transparency using window parameter _NET_WM_WINDOW_OPACITY (eg. using transset). This code implements it back by using the necessary functions from xorg's implementation.

## Disclaimer
I am not experienced at all with X11's API and the X Window System protocol, this was just for me the occasion to discover and modify some code.

Consider this code unreliable.

## Dependencies
* cmake
* a c++ compiler
* xorg development headers
* xorg extension headers (Xrender, Xcomposite, XDamage, Xext)

## Building with cmake
At the root of the project
```
mkdir out
cd out
cmake ../
make 
```

## Copyright
The copyright notice can be found in xcompmgr.cpp file