
***
###Note : What is really do just simple change the import file
import RPi.GPIO as GPIO 
to
import Matrix.GPIO as GPIO

***

Nanopi M1 Matrix-python(edit pin for nanopi m1)
https://github.com/friendlyarm/matrix-python/tree/master/Matrix.GPIO

If you are using other version nanopi, you can reference to
https://github.com/friendlyarm/matrix/blob/master/lib/gpio.c

(default as Nanopi 2 version gpio pins)
https://github.com/friendlyarm/matrix-python/blob/master/Matrix.GPIO/gpio.c

change the matrix-python/Matrix.GPIO/gpio.c pin to your current nanopi corresponding gpio pin..
then install your version of Matrix.GPIO

***

==============
MFRC522-python
==============

A small class to interface with the NFC reader Module MFRC522 on the Nanopi .

This is a Python port of the example code for the NFC module MF522-AN.

##Requirements
This code requires you to have SPI-Py installed from the following repository:
https://github.com/lthiery/SPI-Py

##Examples
This repository includes a couple of examples showing how to read, write, and dump data from a chip. They are thoroughly commented, and should be easy to understand.

## Pins
You can check http://nanopi.io/nanopi-m1.html for reference for Nanopi m1.
If you need other Pi GPIO refernce for FramilyArm site youself.

## You can reference how to connect to RFID RC522 the image in
http://www.theengineeringprojects.com/2015/08/interfacing-rfid-rc522-arduino.html

| Name | Pin # | Pin name   |
|------|-------|------------|
| SDA  | 24    | SPI0_CS/GPIOC3    |
| SCK  | 23    | SPI0_CLK/GPIOC29  |
| MOSI | 19    | SPI0_MOSI/GPIOC0  |
| MISO | 21    | SIP0_MISO/GPIOC1  |
| IRQ  | None  | None              |
| GND  | Any   | Any Ground        |
| RST  | 22    | UART2_RX/GPIOA1   |
| 3.3V | 1     | SYS_3.3V          |

##Usage
Import the class by importing MFRC522 in the top of your script. For more info see the examples.
