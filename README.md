## dwm - dynamic window manager
This is pinosaur's patched version of dwm, the suckless window manager.

The following patches are applied:
- [gaps](https://dwm.suckless.org/patches/gaps/)
- [autostart](https://dwm.suckless.org/patches/autostart/)
- [xresources](https://dwm.suckless.org/patches/autostart/)
- [pertag](https://dwm.suckless.org/patches/pertag/)
- [fakefullscreen](https://dwm.suckless.org/patches/fakefullscreen/)
- [swallow](https://dwm.suckless.org/patches/swallow/)

### Requirements
In order to build dwm you need the Xlib header files.

### Installation (make)
Edit config.mk to match your local setup (dwm is installed into
the /usr/local namespace by default).

Then run
```
make && sudo make clean install
```

### Installation (ebuild)
An ebuild will be available on my website for Gentoo users sometime.
The `savedconfig` and `xinerama` use flags will be available.

### Running dwm
Add the following line to your .xinitrc to start dwm using startx:
```
exec dwm
```
