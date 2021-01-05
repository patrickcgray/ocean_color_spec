# ocean_color_spec

Gear:
Raspberry Pi Zero W
NoIR Camera V2


Burn OS to SD card:
download the Lite version https://www.raspberrypi.org/downloads/raspberry-pi-os/
then burn following instructions herehttps://www.raspberrypi.org/documentation/installation/installing-images/mac.md

Headless Setup:
https://core-electronics.com.au/tutorials/raspberry-pi-zerow-headless-wifi-setup.html
had to run `ping raspberrypi.local` to find IP address (from here https://www.raspberrypi.org/documentation/remote-access/ip-address.md)

Once headless:
follow camera setup here: https://www.raspberrypi.org/documentation/configuration/camera.md

From there instructions at https://blog.durablescope.com/post/BuiltASpectrometer/


---

Instructions for Photodiode based fluorometer

Photodiode is: https://www.adafruit.com/product/1334

Instructions for integration are: https://learn.adafruit.com/adafruit-color-sensors/arduino-code

Code is here: https://github.com/adafruit/Adafruit_CircuitPython_TCS34725/blob/master/adafruit_tcs34725.py

Datasheet for photodiode is: https://cdn-shop.adafruit.com/datasheets/TCS34725.pdf

Set up the rpi zero w as headless

Install circuitpython on the rpi https://learn.adafruit.com/circuitpython-on-raspberrypi-linux/installing-circuitpython-on-raspberry-pi

had to solder a header onto the rpi and then soldered jumpers onto the photodiode


Good example of another project https://diy-fluorometer.github.io/documentation/





