# Plex Raspberry Pi

Using Ansible to get a Raspberry Pi 4 running Raspbian OS

https://www.raspberrypi.org/downloads/raspberry-pi-os/

Raspberry Pi OS (64-bit) Lite

## Pre-req

Advanced OS settings menu

![advanced os menu](doc/images/pi_advanced.png)

Set SSH to Enabled and set user and password

![advanced os settings](doc/images/pi_advanced_options.png)

Add ssh environment vars

```bash
export MEDIAUSER=youruser
export MEDIAPASS=yourpassword
```

## Run

*Don't forget to add your server to the inventory file*

`ansible-navigator run plex_rpi4.yml -i hosts --penv MEDIAUSER MEDIAPASS`

## Sources of help

https://pimylifeup.com/raspberry-pi-plex-server/
