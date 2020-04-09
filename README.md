# BioStamp3™ Firmware Images

This repository contains BioStamp3™ firmware image files.

## 2020-04-09 - [brc3app_8f61a128.img][1]

  * Fixed a crash that occurred when BLE disconnects while a command is in progress
  * Changed I2C bus speed from 400kHz to 250kHz to avoid an errata that caused the 400kHz timing to be very slightly out of spec
  * Modified memory usage to enable any combination of sensors, including all sensors at once, without crashing
  * Modified AD5940 calibration process

[1]: https://raw.githubusercontent.com/MC10Inc/biostamp-firmware/master/images/brc3app_8f61a128.img