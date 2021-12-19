# ocean_color_spec

### Ocean Color Spec 2.0
Using a Raspberry Pi 3B+ and the Adafruit AS7341 10-Channel Light / Color Sensor Breakout. Followed the instructions from: https://learn.adafruit.com/adafruit-as7341-10-channel-light-color-sensor-breakout to set it up, wire it in, and get the software running in python. This took my Pi over an hour to update and get everything installed so worth running this before you're properly caffienated and ready to make/hack.

Overall goal is to have a system with three of these AS7341 sensors. One looking at the water, one at the sky, and one at a calibrated irradiance plaque (or a cheap 18% photographers grey card) in order to make calibrated measurements of ocean color. If used on a ship this system could be upgraded with a gimbal to get much more consistent measurements of Rrs with roll and pitch held constant.

I will 3D print the housing to hold all three sensors, the plaque, and the raspberry pi in the correct viewing geometry. I'll possibly use a gimbal to hold it stable. I want to test the sensors for consistency across each other, uncertainty in time when viewing a consistent surface, and sensitivity to actually measuring ocean color considering how dark the water can be. A fourth sensor could be used for an in-situ calibrator if this is used on a fixed platform. Regardless I'd like to compare this to measurements made with the skylight blocked approach.





### Initial Try:
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





