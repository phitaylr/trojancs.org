---
title: "Switches and Distance Finders"
date: 2021-02
draft: false
---


# SWITCHES

My goal was to use the pushbutton as a switch, so that when you pressed down, the output would change and wouldn't change again until the button was released and then pressed again. 

```
bool buttonPressed = false;
bool beenPressed = false;
bool flashing = false;

void loop() {

  if (digitalRead(2) == LOW) {
    buttonPressed = true;
  } else {
    buttonPressed = false;
    beenPressed = false;
  }

  if (buttonPressed == true && beenPressed == false) {
    flashing = !flashing;
    beenPressed = true;
  }
```
Everytime the signal from PIN 2 *changes* from LOW to HIGH, the boolean (```flashing```) switches. To detect when it changes, I used a variable to keep track of what the signal was on the last loop. If that variable is LOW and the current one is HIGH, then the boolean switches.


# Range Finders

So basically I learned how ultrasonic distance sensors work. A short signal gets send to the distance sensor. When the sensor receives it, it sensor sends out a freq that will go out, bounce off something, and return. When they return, a the sensor will send back a signal. If the object is farther away, it will take longer for the waves to hit it and bounce back, so it will take longer to send the return signal. So depending on how long the signal takes to come back, you can find how far away the object is.

So basically here:

*tinkercad photo*

