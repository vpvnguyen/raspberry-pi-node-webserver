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
- Go to https://nodejs.org/en/download/
- Download version specific to your Raspberry Pi's ARM

<!-- server {
        listen 80 default_server;
        listen [::]:80 default_server;

        root /var/www/html;

        index index.html index.htm index.nginx-debian.html;

        server_name _;

        location / {
                proxy_pass http://localhost:3000;
                proxy_http_version 1.1;
                proxy_set_header Upgrade $http_upgrade;
                proxy_set_header Connection 'upgrade';
                proxy_set_header Host $host;
                proxy_cache_bypass $http_upgrade;
        }
} -->
