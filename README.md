# Plex Raspberry Pi

Using Ansible to get a Raspberry Pi 4 running Raspbian OS

https://www.raspberrypi.org/downloads/raspberry-pi-os/

Raspberry Pi OS (32-bit) Lite

https://pimylifeup.com/raspberry-pi-plex-server/


##static ip, instead of doing this on the pie, maybe set with the mac on the router instead?
###add lines to file /etc/dhcpcd.conf
```
interface eth0

static ip_address=192.168.4.2/24
static routers=192.168.4.1
static domain_name_servers=192.168.4.1
```

##enable ssh
```
systemctl enable ssh
systemctl start ssh
```