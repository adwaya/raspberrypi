# RaspberryPi
The Raspberry Pi is a tiny and affordable computer that you can use to learn programming and practical projects.

## Installing OS on RaspberryPi

Get an SD card and format it using SDcard formatter, the application can be downloaded from `https://www.sdcard.org/downloads/formatter_4/` 

![](/images/SDCardFormatting.png)

*NOOBS* is an easy operating system installer which contains Raspbian. It also provides a selection of alternative operating systems which are then downloaded from the internet and installed.

Download the *NOOBS* OS and install onto the SD Card `https://www.raspberrypi.org/downloads/noobs/` and download the *Offline ZIP*

Extract the *ZIP* and copy/paste onto the formatted SD card, now the *HDD Storage* is ready!!!

##Connecting to the Display
Now, place the SD card in the RaspberryPi slot, connect the HDMI cable, keyboard and mouse to the USB slots.
Power ON the raspberry device with the microUSB connector.
![](/images/BootingGreenLight.png)

##Login to the OS

Raspberry Pi uses `pi` as the username and `raspberry` as the password for the login.
To go to the configuration page for the OS like boot menu, type `raspi-config` on the console
To enable *SSH* access to raspberry pi, goto `rasp-config` -> `Interfacing Options` ->  `SSH`
To connect using SSH using remote computer , use `pi@<ip>` 
**Note**: IPaddress`<ip>` of the raspberryPi and the remote computer should be on the same network.

##Installing application on RaspberryPi

**Apache Installation**
- `apt update` and `apt install apache2` to install apache.
- check the application working in the browser <ip>:80
**Jenkins Installation**
- Run apt-get updateand wait for it to get completed
Run wget -q -O - https://pkg.jenkins.io/debian/jenkins-ci.org.key | sudo apt-key add - to add the key and this should return OK
Then Run sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list' , this command will add the URL to the sources list.
Now install jenkins using apt-get install jenkins and wait till it gets completed.
**Docker Installation** :whale:
Install Docker using following command `curl -sSL https://get.docker.com | sh`
Add “pi” user to “docker” group using the following command `sudo usermod -aG docker pi`
