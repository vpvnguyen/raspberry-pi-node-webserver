# Node.js webserver for Raspberry Pi 3
The intention of this product is to create a Node.js webserver on your raspberry 3 as a developmental server.

# Requirements
- Raspberry Pi 3
- 8gb SD card

# Setup - Raspberry Pi
- Format SD card.
- Recommended for MacOSX: https://www.sdcard.org/downloads/formatter/
- Install Raspian via NOOBS or terminal on to an SD card.
- src: https://www.raspberrypi.org/downloads/
- Insert SD card into Raspberry Pi and boot it.
> When the Raspberry Pi boots, a grey screen with image options are listed. Raspian with Desktop is the one used in this setup.
> Installation can take 45+ mins.

# Setup - Node.js Server
### Install in Raspian
- Boot into Raspian.
- Navigate to Preferences > Raspberry Pi Configuration
- Enable VNC
- Check ARM version
- Terminal: `uname -m`
- Go to https://nodejs.org/en/download/
- Download version specific to your Raspberry Pi's ARM
### Over SSH
- SSH must be enabled on raspberry pi
- SSH into pi `ssh pi@<ip_address>`
- Visit [NodeSource](https://github.com/nodesource/distributions/blob/master/README.md) for latest release
- Update package manager `sudo apt update`
- Follow instructions to install using curl

# vscode
- Open raspberry pi terminal
- Remove any failing build: `sudo apt-get purge code-oss`
- Install downgraded working version: `sudo apt-get install code-oss=1.29.0-1539702286`
- Prevent auto update: `sudo apt-mark hold code-oss`
- UNDO prevent auto update: `sudo apt-mark unhold code-oss`

# plex
- Follow: https://support.plex.tv/articles/200288586-installation/#toc-1
- Download installer
- cd into installer dir
- `sudo dpkg -i <DOWNLOADED_FILENAME>.deb`
- Configure at: http://127.0.0.1:32400/web
