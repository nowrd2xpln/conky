# Conky Configuration Files
My collection of conky config files.

## Getting started
These instruction will provide information on installation and templates to drop into your home directory. Initially this project is targeted for using the Raspberry Pi 3 B+ to manage serial port connections.

### HW/OS Environment
This conky setup and configuration has been tested with the following hardware and operating systems:

Raspberry Pi 3 with Ubuntu Mate 16.4.02 (Xenial)
'''
$ cat /proc/cpuinfo
processor       : 0
model name      : ARMv7 Processor rev 4 (v7l)
BogoMIPS        : 76.80
Features        : half thumb fastmult vfp edsp neon vfpv3 tls vfpv4 idiva idivt vfpd32 lpae evtstrm crc32
CPU implementer : 0x41
CPU architecture: 7
CPU variant     : 0x0
CPU part        : 0xd03
CPU revision    : 4
Hardware        : BCM2709
Revision        : a22082
Serial          : 00000000bca4b753

$ cat /etc/os-release
NAME="Ubuntu"
VERSION="16.04.2 LTS (Xenial Xerus)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 16.04.2 LTS"
VERSION_ID="16.04"
HOME_URL="http://www.ubuntu.com/"
SUPPORT_URL="http://help.ubuntu.com/"
BUG_REPORT_URL="http://bugs.launchpad.net/ubuntu/"
VERSION_CODENAME=xenial
UBUNTU_CODENAME=xenial
'''

Raspberry Pi 3 B+ with Raspbian Stretch with Desktop
'''
$ cat /proc/cpuinfo
model name      : ARMv7 Processor rev 4 (v7l)
BogoMIPS        : 89.60
Features        : half thumb fastmult vfp edsp neon vfpv3 tls vfpv4 idiva idivt vfpd32 lpae evtstrm crc32
CPU implementer : 0x41
CPU architecture: 7
CPU variant     : 0x0
CPU part        : 0xd03
CPU revision    : 4
Hardware        : BCM2835
Revision        : a020d3
Serial          : 00000000a3d22477

$ cat /etc/os-release
PRETTY_NAME="Raspbian GNU/Linux 9 (stretch)"
NAME="Raspbian GNU/Linux"
VERSION_ID="9"
VERSION="9 (stretch)"
ID=raspbian
ID_LIKE=debian
HOME_URL="http://www.raspbian.org/"
SUPPORT_URL="http://www.raspbian.org/RaspbianForums"
BUG_REPORT_URL="http://www.raspbian.org/RaspbianBugs"
'''

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
$> wget -O /usr/bin/conky.sh https://raw.githubusercontent.com/nowrd2xpln/conky/master/conky.sh
```
Download the file used for the autostart process into /etc/xdg/autostart/
```
$> wget -O /etc/xdg/autostart/conky.desktop https://raw.githubusercontent.com/nowrd2xpln/conky/master/conky.desktop
```
Reboot the system

