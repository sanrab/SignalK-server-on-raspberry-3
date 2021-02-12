# SignalK-server-on-raspberry-3
SignalK server on raspberry 3

install RaspiOS Lite
sudo raspi-config (server name, password, locale, time zone, keyboard)
sudo apt update
sudo apt install nodejs npm
sudo npm install -g npm@latest
sudo apt install libnss-mdns avahi-utils libavahi-compat-libdnssd-dev (AVAHI BONJOUR)
sudo npm install -g --unsafe-perm signalk-server
CHECK
signalk-server --sample-nmea0183-data

sudo signalk-server-setup

sudo systemctl enable signalk.service
sudo systemctl enable signalk.socket

