
## Controlling Servo using Potentiometer:
### Problem Statement:
The aim of the simulation is to rotate a servo motor based on the readings of a potentiometer. 

### Description:
A servo motor is a special kind of DC motor which provides us precise control in terms of angular position or linear position. We control the exact angle of rotation of the servo motor using the data that we have collected using the Potentiometer. Potentiometer is like a analog device which gives us anlaog data based on the rotation of the nob present in it. It is the same that is present in the fan regulators.

### Components:
1. Arduino Uno
2. Positional Micro Servo
3. 250 kΩ Potentiometer

### Optional:
[How does servo works?](https://www.tutorialspoint.com/arduino/arduino_servo_motor.htm)

### Schematic:
![diagram](./images/Screenshot%20from%202020-12-24%2017-08-59.png)

### Code:
```
/* Controlling a servo position using a potentiometer (variable resistor) */

#include <Servo.h>
   Servo myservo; // create servo object
    // analog pin used to connect the potentiometer
   int val; // variable to read the value from the analog pin

void setup() {
   myservo.attach(2); // attaches the servo on pin 2 to the servo object
   pinMode(A0, INPUT);

}

void loop() {
   val = analogRead(A0);
   // reads the value of the potentiometer (value between 0 and 1023)
   val = map(val, 0, 1023, 0, 180);
   // scale it to use it with the servo (value between 0 and 180)
   myservo.write(val); // sets the servo position according to the scaled value
   delay(15);
}
```
### Link to TinkerCAD:
[Link](https://www.tinkercad.com/things/gE6u7EHe2Jy)
