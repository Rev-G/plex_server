# Plex Raspberry Pi

Using Ansible to get a Raspberry Pi 4 running Raspbian OS

https://www.raspberrypi.org/downloads/raspberry-pi-os/

Raspberry Pi OS (64-bit) Lite

1. pre-req
    1. OS setup with ssh enabled
1. add ssh user environment var `export MEDIAUSER=youruser`
1. add ssh password environment var `export MEDIAPASS=yourpassword`
1. add the pi server to the "hosts" file
1. run `ansible-navigator run plex_rpi4.yml -i hosts --penv MEDIAUSER MEDIAPASS`

https://pimylifeup.com/raspberry-pi-plex-server/
