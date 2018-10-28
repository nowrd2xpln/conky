# Conky Configuration Files
My collection of conky config files.

## Getting started
These instruction will provide information on installation and templates to drop into your home directory. Initially this project is targeted for using the Raspberry Pi 3 B+ to manage serial port connections.

### HW/OS Environment
Raspberry Pi 3 B+

PRETTY_NAME="Raspbian GNU/Linux 9 (stretch)"
NAME="Raspbian GNU/Linux"

VERSION_ID="9"

VERSION="9 (stretch)"

ID=raspbian

ID_LIKE=debian 
HOME_URL="http://www.raspbian.org/" 

### Install
Install conky
```
sudo apt-get -y install conky
```
Download the conky configuration file to your home directory
```
$> wget -O ~/.conkyrc https://raw.githubusercontent.com/nowrd2xpln/conky/master/rpi/.conkyrc
```
Download the shell script to /usr/bin/conky.sh
```
$> wget -O /usr/bin/conky.sh https://raw.githubusercontent.com/nowrd2xpln/conky/master/conky.rc
```
Download the file used for the autostart process into /etc/xdg/autostart/
```
$> wget -O /etc/xdg/autostart/conky.desktop https://raw.githubusercontent.com/nowrd2xpln/conky/master/conky.desktop
```
Reboot the system

