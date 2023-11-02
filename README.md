# raspi_dev
Setup for raspberry pi development system

The premise for most performance "enhancements" is to actual remove things that eat up IO.


## Software

VS Code
`sudo apt-get install code`



## Performance Enhancements

`sudo swapoff -a`  disables swap memory; unnecessary and unneeded wear&tear on SD card

`boot/cmdline.txt`
- change tty1 to tty3
- append `loglevel=3 quiet logo.nologo` at the end after `rootwait`


## Potential Enhancements

`sudo systemctl disable wifi-country.service`  need to test if this works for I18N folks

`sudo systemctl disable triggerhappy.service`  disable joystick support

`sudo systemctl disable hciuart.service`  disable Blueteeth
