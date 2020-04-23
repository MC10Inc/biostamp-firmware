# BioStamp3™ Firmware Images

This repository contains BioStamp3™ firmware image files.

This firmware adds a new option to configure the AFE4900 sampling rate in all modes (ECG, PPG, SpO2). The option is mandatory so the existing Android and web apps which don't have it yet will not be able to enable the AFE4900 in any mode. The attached Android app adds that setting internally so that it will continue to work in ECG mode, but it does not yet have any support for PPG otherwise.

## 2020-04-28 - [brc3app_e7a04a70.img][3]

  * Add SpO2 mode (red + IR) for AFE4900
  * Stop recording when flash memory is full

## 2020-04-13 - [brc3app_c6b1227a.img][2]

  * Increase BLE TX power from 0dBm to +4dBm
  * Stop sensing when memory is full
  * Add status broadcast to advertisements

## 2020-04-09 - [brc3app_8f61a128.img][1]

  * Fix a crash that occurred when BLE disconnects while a command is in progress
  * Change I2C bus speed from 400kHz to 250kHz to avoid an errata that caused the 400kHz timing to be very slightly out of spec
  * Modify memory usage to enable any combination of sensors, including all sensors at once, without crashing
  * Modify AD5940 calibration process

[1]: https://raw.githubusercontent.com/MC10Inc/biostamp-firmware/master/images/brc3app_8f61a128.img
[2]: https://raw.githubusercontent.com/MC10Inc/biostamp-firmware/master/images/brc3app_c6b1227a.img
[3]: https://raw.githubusercontent.com/MC10Inc/biostamp-firmware/master/images/brc3app_e7a04a70.img
