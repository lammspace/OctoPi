# LAMM OctoPi Software Docs

## Starting point

* Raspberry Pi 3
* Target SD card

## Initial setup

1. Download image from http://octoprint.org/download/
2. Insert SD card into pc
3. Delete any existing partitions with gparted
4. Run `sudo dd bs=4M if=octopi.img of=/dev/sdb` where octopi.img is the image and /dev/sdb is the location of the sd
5. Once the writing is complete, eject and re-insert the SD card
6. Use gparted to expand the ext4 partition to use up the rest of the unoccupied space
7. Eject SD card and insert it into the Pi
8. Boot the Pi
9. Ssh into pi@octopi.local. The default username is raspberry
10. Change the password with passwd, and record the new credentials in a secure location
11. Run `sudo hostname targethostname` to change the hostname
12. navigate to octopi.local in a browser and setup access credentials for the web interface
