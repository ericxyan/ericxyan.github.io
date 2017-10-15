Command
====================
1. Add new user
````
# Add a user: eric and create home directory /home/eric
useradd -m eric 
# add to sudoers
sudo usermod -aG sudo eric
# NOpasswd
GROUPERIC	ALL = NOPASSWD: /usr/bin/updatedb, PASSWD: /bin/kill
# check privilege
sudo -l
# repeat last cmd
sudo !!
# cache sudo password
sudo -v
# clean cache
sudo -k
````
