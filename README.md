backlight-openrc
================

Save the screen light settings at shutdown and restore it at boot time, using OpenRC init scripts.

# Installation
### Arch Linux Based
1. Install the package using the [AUR tar ball](https://aur.archlinux.org/404)

### Non Arch Linux Based
1. Clone this repo
2. Copy the file **backlight** in */etc/init.d/*
3. Give it the right permission with
`# chown root:root /etc/init.d/backlight; chmod 755 /etc/init.d/backlight`

# Setup
After installing you should add the service to the system boot schedule with
`# rc-update add backlight boot`

# How-to uninstall
### Arch Linux Based
1. `# pacman -Rs backlight-openrc`

### Non Arch Linux Based
1. `# rm /etc/init.d/backlight`
2. `# rc-update del backlight boot`
