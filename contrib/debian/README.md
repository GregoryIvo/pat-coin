
Debian
====================
This directory contains files used to package patriotcoind/patriotcoin-qt
for Debian-based Linux systems. If you compile patriotcoind/patriotcoin-qt yourself, there are some useful files here.

## patriotcoin: URI support ##


patriotcoin-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install patriotcoin-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your patriotcoin-qt binary to `/usr/bin`
and the `../../share/pixmaps/patriotcoin128.png` to `/usr/share/pixmaps`

patriotcoin-qt.protocol (KDE)

