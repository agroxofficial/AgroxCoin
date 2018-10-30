
Debian
====================
This directory contains files used to package agroxd/agrox-qt
for Debian-based Linux systems. If you compile agroxd/agrox-qt yourself, there are some useful files here.

## agrox: URI support ##


agrox-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install agrox-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your agroxqt binary to `/usr/bin`
and the `../../share/pixmaps/agrox128.png` to `/usr/share/pixmaps`

agrox-qt.protocol (KDE)

