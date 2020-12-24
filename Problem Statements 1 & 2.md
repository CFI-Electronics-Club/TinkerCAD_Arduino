# Problem statements #

### Introduction: 

I hope most of you would have attended the live session. If not, fret not. Just go through the "[Main Readme.MD](https://github.com/CFI-Electronics-Club/TinkerCAD_Arduino/blob/main/README.md)". That would give you some information about TinkerCAD and the instructions. Once you have practiced working with the environment, you can solve the Problem statements on your own.

## Problem statement 1: Blinking an in-built LED (Pin 13):

In the Arduino board, there is an in-built LED which is present to indicate whether the power supply is proper and the board is properly functioning. Since, we are just now starting on, the PS is simple. Just blink that LED periodically, i.e., switch it on for first half of the period and switch it off in the next half. (Take the period as 10 seconds). 

**Disclaimer**: The solution is contained below. If you like to do it on your own, please try to do it and then if you are stuck, check the solution provided. 

1. LED is blinking
![temp](https://github.com/CFI-Electronics-Club/TinkerCAD_Arduino/blob/main/images/p1(1).jpg)

2. LED ain't blinking:
![temp](https://github.com/CFI-Electronics-Club/TinkerCAD_Arduino/blob/main/images/p1(2).jpg)

3. Arduino code:

![temp](https://github.com/CFI-Electronics-Club/TinkerCAD_Arduino/blob/main/images/p1(3).jpg)

### Solution:
As you could see from the pictures, the solution is really simple. Just configure the digital pin 13 to be HIGH and LOW for the required time intervals. No external circuitry needed since we are after all, blinking an in-built LED.

_________________________________________________________________________________________________________________________________________________________________________________

## Problem statement 2: Blinking an external LED:

This PS is very much similar to the previous PS except that now you should blink an LED which is externally connected to the Arduino board periodically for 10 seconds with it being ON for the first five seconds and OFF for the next five seconds.

**Disclaimer**: The solution is contained below. If you like to do it on your own, please try to do it and then if you are stuck, check the solution provided.

1. LED is blinking
![temp](https://github.com/CFI-Electronics-Club/TinkerCAD_Arduino/blob/main/images/p2(1).jpg)

2. LED ain't blinking:
![temp](https://github.com/CFI-Electronics-Club/TinkerCAD_Arduino/blob/main/images/p2(2).jpg)

3. Arduino code:

![temp](https://github.com/CFI-Electronics-Club/TinkerCAD_Arduino/blob/main/images/p2(3).jpg)

### Solution:
The code is mostly the same code used in the previous PS. Infact, only the pin number is changed from 9 to 13 since the anode is connected to pin 9 across a resistor. You could even use pin 13 itself for the purpose. Pin 13 is special because it also controls the internal LED. Coming to the external circuitry, what is done is the cathode is directly connected to Ground(**GND**) or logical LOW. The anode is connected to pin 9 via a resistor. Such a resistor is known as a current controlling resistor which prevents a very high current from flowing into the LED and hence, prevents it from being damaged.

## Links to the TinkerCAD circuits:

[Blinking an in-built LED (Pin 13)](https://www.tinkercad.com/things/buVfr3nr1CD-blinking-an-in-built-led/editel?sharecode=ANGtTLGq9eGByxeh_qvNuvi1ZTnO_AKegXDY-5uDa-s)
[Blinking an external LED](https://www.tinkercad.com/things/gkocusjLsds-blinking-an-external-led/editel?sharecode=cVtirfTHw1lSKSDOYF22_H1mT32WZrt19SsBkdlDRAs)
