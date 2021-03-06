# raspbian-arm64
How to install a 64-bit version of Raspbian on a Raspberry Pi 4

## High level steps
1. Download a image of Raspbian 64-bit
1. Flash the image to a Raspberry Pi bootable media
1. Follow the normal Raspbian installation steps

### Download a Raspbian 64-bit image
Please see the following resources,
* [Initial Beta Test Announcement](https://www.raspberrypi.org/forums/viewtopic.php?t=275370)
* [Forum Feedback Thread](https://www.raspberrypi.org/forums/viewtopic.php?f=63&t=275372)
* [Known Issue List](https://github.com/raspberrypi/Raspberry-Pi-OS-64bit/issues)

The latest image can be found in this forum post,
https://www.raspberrypi.org/forums/viewtopic.php?f=63&t=275372&start=250#p1717623

### Flashing the 64-bit Raspbian image
I used the new Raspberry Pi Imager located here, https://www.raspberrypi.org/software/

### Installation
From this point the installation follows the same process as the 32-bit version of Raspbian.

## Additional Setup for Owncloud and PiHole

### Install latest Docker
I used the covienence script to install the latest and greatest version of Docker,
https://docs.docker.com/engine/install/debian/#install-using-the-convenience-script

### Update Rasbian 64-bit with Python Dependencies
If you try to ```pip3 install docker-compose``` at this point it will fail with missing dependencies, to fix it follow this page,
https://github.com/pyenv/pyenv/wiki/Common-build-problems

### Install latest docker-compose
Now ```pip3 install docker-compose``` will work.
