# Ardupilot_External_LEDs

## Description

This project is expand UAV External LEDs and easy DIY, This WS2812 LED controller communitcate with ardupilot with I2C, support Ardupilot firmware ver 3.6 and higher, only test with multicopters, others like Rover, Plane not have test. LEDs only for the popular WS2812, aka Neopixel， only support 3 LEDs every channel.

* LED controller: STM32F103 or Arduino pro mini
* LED type: WS2812
* Muti-channel: 4~8 or more
* Features: 2 channels for navigation, blinking with red color, others sync with pixhawk main LED status. ref ardupilot wiki page [LED Meaning](https://ardupilot.org/copter/docs/common-leds-pixhawk.html)
* Ardupilot firmware version: 3.6 and higher


## Hardware

* STM32 Bluepill or STM32 Blackpill
* Arduino Pro mini 3.3V 8MHz or 5V 16MHz

### Wrie

| Board  | Pin | comments    |
|:-------|:---|:-----------|
| STM32 bluepill or blackpill  | PA0 | for drone heading, always blinking RED color   | 
|  | PA1  | for sync status with ardupilot main LED status      |
| Arduino Pro mini  | D8   | for drone heading, always blinking RED color |
|		|  D9 | sync ardupilot main LED status	|	


## Firmware
| Board | Firmware name|
|:----|:-----|
| STM32 bluepill or blackpill |  APM_EXTERNAL_LED_COM_V2.0.4.bin |
| Arduino Pro mini 3.3V 8MHz | APM_EXTERNAL_LED_COM_Arduino_8HMz_V1.0.1.hex |
| Arduino Pro mini 5V 16MHz | APM_EXTERNAL_LED_COM_Arduino_16MHz_V1.0.1.hex |
