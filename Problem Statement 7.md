**Problem Statement:**

Attach a Photo resistor and use them to control the brightness of a led.

**Components:**
1. Arduino UNO
2. LED
3. Resistors
4. Photoresistor 

**Circuit:**

![](https://github.com/Snehan2k2/TinkerCAD_Arduino/blob/patch-1/images/p7.png)

**Code:**
`<
int sensorValue = 0;

void setup()
{
  pinMode(A0, INPUT);
  Serial.begin(9600);

  pinMode(9, OUTPUT);
}

void loop()
{
  // read the value from the sensor
  sensorValue = analogRead(A0);
  // print the sensor reading so you know its range
  Serial.println(sensorValue);
  // map the sensor reading to a range for the LED
  analogWrite(9, map(sensorValue, 0, 1023, 0, 255));
  delay(100); // Wait for 100 millisecond(s)
}
>`

[Link for the Simulation](https://www.tinkercad.com/things/9fsyf0X0Qg5-daring-bigery-jaagub/editel)
