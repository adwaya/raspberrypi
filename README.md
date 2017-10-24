#RaspberryPi
-The Raspberry Pi is a tiny and affordable computer that you can use to learn programming and practical projects.

##Installing OS on RaspberryPi

Grab a SD card and format it using the application, the application can be downloaded from `https://www.sdcard.org/downloads/formatter_4/`

*NOOBS* is an easy operating system installer which contains Raspbian. It also provides a selection of alternative operating systems which are then downloaded from the internet and installed.

Download the *NOOBS* OS and install onto the SD Card `https://www.raspberrypi.org/downloads/noobs/` and download the *Offline ZIP*

Extract the *ZIP* and copy/paste onto the formatted SD card, now the *HDD Storage* is ready!!!

##Connecting to the Display
Now, place the SD card in the RaspberryPi slot, connect the HDMI cable, keyboard and mouse to the USB slots.
Power ON the raspberry device with the microUSB connector.

##Login to the OS

Raspberry Pi uses `pi` as the username and `raspberry` as the password for the login.
To go to the configuration page for the OS like boot menu, type `raspi-config` on the console
To enable *SSH* access to raspberry pi, goto `rasp-config` -> `Interfacing Options` ->  `SSH`
To connect using SSH using remote computer , use `pi@<ip>` 
**Note**: IPaddress`<ip>` of the raspberryPi and the remote computer should be on the same network.
