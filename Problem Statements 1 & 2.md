# Problem statements #

Introduction: 

I hope most of you would have attended the live session. If not, fret not. Just go through the "[Main Readme.MD](https://github.com/CFI-Electronics-Club/TinkerCAD_Arduino/blob/main/README.md)". That would give you some information about TinkerCAD and the instructions. Once you have practiced working with the environment, you can solve the Problem statements on your own.

## Problem statement 1: Blinking an in-built LED (Pin 13):

In the Arduino board, there is an in-built LED which is present to indicate whether the power supply is proper and the board is properly functioning. Since, we are just now starting on, the PS is simple. Just blink that LED periodically, i.e., switch it on for first half of the period and switch it off in the next half. (Take the period as 10 seconds).

1. LED is blinking
![temp](https://github.com/CFI-Electronics-Club/TinkerCAD_Arduino/blob/main/images/p1(1).jpg)

2. LED ain't blinking:
![temp](https://github.com/CFI-Electronics-Club/TinkerCAD_Arduino/blob/main/images/p1(2).jpg)

3. Arduino code:
![temp](https://github.com/CFI-Electronics-Club/TinkerCAD_Arduino/blob/main/images/p1(3).jpg)

### Solution:
As you could see from the pictures, the solution is really simple. Just configure the digital pin 13 to be HIGH and LOW for the required time intervals. No external circuitry needed since we are after all, blinking an in-built LED.

___________________________________________________________________________________________________________________________________________________________________________________

## Problem statement 2: Blinking an external LED:

This PS is very much similar to the previous PS except that now you should blink an LED which is externally connected to the Arduino board periodically for 10 seconds with it being ON for the first five seconds and OFF for the next five seconds.
