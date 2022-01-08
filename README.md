# e-Ink Display Home Assistant

A Waveshare 4.2" e-ink display for viewing sensors data from Home Assistant. The firmware is based on ESPHome. I take inspiration from <b>MaxMac_STN</b>'s work (https://github.com/maxmacstn/HA-ePaper-Display), especially for the hardware and the 3D-printed case.

![header](https://github.com/sainz/Home-Assistant-e-Ink-Display/blob/master/images/PXL_20220108_093319359.jpg?raw=true)


### Hardware
I bought the display and ESP8266 on Amazon, but you can easily find both on Aliexpress or Bangood. Following the Amazon.it links for both parts (affiliated links)
- Waveshare 4.2inch E-paper Display Module: https://amzn.to/3ESIhD4
- Wemos D1 Mini ESP8266: https://amzn.to/3EQsyEu

You'll have to solder all wires diretly on both display and board. Check the <b>MaxMac_STN</b>'s Github page for the connection schema and the tutorial. You'll find the .stl files for the 3D-Printed Case too.


### Installation
- You need an Home Assistant installation with ESPHome add-on installed;
- I create some text sensor, to easly adapt them for the e-Ink Display (check sensors.yaml). This file is linked to configuration.yaml of Home Assistant installation. You must adapt it based on your sensors data;
- Copy fonts folder on your ESPHome folder
- After connect all the hardware together, link it to Home Assistant and flash the firmware (epaper-display.yaml). This is my personal configuratio, so you must adaopt based on your Home Assistant configuration and sensors data.

N.B.: always flash the firmware via USB, not by OTA.
