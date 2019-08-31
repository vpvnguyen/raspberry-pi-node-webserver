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
- Boot into Raspian.
- Navigate to Preferences > Raspberry Pi Configuration
- Enable VNC
- Check ARM version
- Terminal: `uname -m`
