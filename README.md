# Plex Raspberry Pi

Using Ansible to get a Raspberry Pi 4 running Raspbian OS

https://www.raspberrypi.org/downloads/raspberry-pi-os/

Raspberry Pi OS (32-bit) Lite

1. create ssh key on local system using `ssh-keygen`
1. boot respberry pi
1. sudo raspi-config
    - Interfacing Options > SSH > Enable
    - Localisation Options > Update all locals
1. reboot the pi using `sudo reboot`
1. use `ssh-copy-id -i ~/.ssh/mykey user@host` to put your key on the raspberrypi
1. test ssh 
1. create virtual python3 env `python3 -m venv vansible`
1. use virtual env `source vansible/bin/activate`
1. install ansible `pip3 install ansible`
1. add ssh user environment var `export SSH_USER=yourpiuser`
1. add the pi server to the "hosts" file
1. run `ansible-playbook -i hosts plex_rpi4.yml`

https://pimylifeup.com/raspberry-pi-plex-server/

https://github.com/Rev-G/plex_server.git

ansible-playbook plex_rpi4.xml --ask-become-pass