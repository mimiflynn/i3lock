Animated Screen Locker
===============================
![examples of it working](http://thumbs.gfycat.com/QuaintAnchoredBoaconstrictor-size_restricted.gif)

I3Locker, with your keypresses animating the screen!

Adds a -a format which specifies where to pull animation files from. Animation files must be in .png format. 

Example Usage, to see the gif: ./i3lock -i ./imgs/wallpaper/ed-wallpaper.png -a imgs/

A fork from https://github.com/i3/i3lock . See the README there as well.

=======
- i3lock uses PAM and therefore is compatible with LDAP etc.
  On OpenBSD i3lock uses the bsd_auth(3) framework.

Requirements
------------
- pkg-config
- libxcb
- libxcb-util
- libpam-dev
- libcairo-dev
- libxcb-xinerama
- libev
- libx11-dev
- libx11-xcb-dev
- libxkbcommon >= 0.5.0
- libxkbcommon-x11 >= 0.5.0

Running i3lock
-------------
Simply invoke the 'i3lock' command. To get out of it, enter your password and
press enter.

On OpenBSD the `i3lock` binary needs to be setgid `auth` to call the
authentication helpers, e.g. `/usr/libexec/auth/login_passwd`.

Upstream
--------
Please submit pull requests to https://github.com/i3/i3lock


## Ubuntu build notes

```
libxkbcommon-x11-dev
libxkbcommon-dev
libexcb-xinerama0-dev
libxcb-util-dev
libxcb-xkb-dev
libpam0g-dev
libcairo2-dev
libev-dev
libx11-xcb-dev
libx11-dev
libxinerama-dev
libxcb-dpms0-dev
libxcb-image0-dev
```
