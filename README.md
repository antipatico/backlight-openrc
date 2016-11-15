backlight-openrc
================

Save the screen light settings at shutdown and restore it at boot time, using OpenRC init scripts.

# Installation
### Arch Linux Based
1. Install the package using the [AUR tar ball](https://aur.archlinux.org/packages/backlight-openrc/)

### Non Arch Linux Based
1. Clone this repo
2. Install the file **backlight** in */etc/init.d/* with
```bash
install -m=755 -oroot backlight /etc/init.d/backlight
```

# Setup
After installing you should add the service to the system boot schedule with
```bash
rc-update add backlight
```

# How-to uninstall
### Arch Linux Based
1. Just remove it with pacman
```bash
pacman -R backlight-openrc
```

### Non Arch Linux Based
1. First remove it from the system startup
```bash
rc-update del backlight -a
```
2. Then just delete the script from your system
```bash
 rm /etc/init.d/backlight
```
