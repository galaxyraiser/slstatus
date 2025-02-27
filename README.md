**slstatus - suckless status**
==========================
slstatus is a suckless status monitor for window managers that use WM_NAME
(e.g. dwm) or stdin to fill the status bar.


**Features**
--------
- Battery percentage/state/time left
- CPU usage
- CPU frequency
- Custom shell commands
- Date and time
- Disk status (free storage, percentage, total storage and used storage)
- Available entropy
- Username/GID/UID
- Hostname
- IP address (IPv4 and IPv6)
- Kernel version
- Keyboard indicators
- Keymap
- Load average
- Network speeds (RX and TX)
- Number of files in a directory (hint: Maildir)
- Memory status (free memory, percentage, total memory and used memory)
- Swap status (free swap, percentage, total swap and used swap)
- Temperature
- Uptime
- Volume percentage (OSS/ALSA)
- WiFi signal percentage and ESSID


**Requirements**
------------
Currently slstatus works on FreeBSD, Linux and OpenBSD.
In order to build slstatus you need the Xlib header files.

If you will not change nothing of this configuration, you will also need to install the following utilities:
```
1. acpilight
2. alsa
```
IT'S POSSIBLE THAT YOU NEED TO CHANGE THE VALUE OF THE CONSTANT **"bat"** in case you use a laptop and
its battery file has not fond at **/sys/class/power_supply/BAT0.** Usually the value of this is: **BAT0** or **BAT1.**

If you want to use "the weather view feature" you need to install [ansiweather](https://github.com/brookiestein/ansiweather) 
which is developed by [fcambus](https://github.com/fcambus).

Installation
------------
Edit config.mk to match your local setup (slstatus is installed into the
/usr/local namespace by default).

Afterwards enter the following command to build and install slstatus (if
necessary as root):

    make clean install


Running slstatus
----------------
See the man page for details.


Configuration
-------------
slstatus can be customized by creating a custom config.h and (re)compiling the
source code. This keeps it fast, secure and simple.

Todo
----
Cleaning up the whole codebase it the goal before thinking about a release.

**Fonts**
---------
https://gist.github.com/matthewjberger/7dd7e079f282f8138a9dc3b045ebefa0
