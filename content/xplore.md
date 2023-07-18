---
title: "Xplore"
draft: false
bookToC: true
---

# Tuesday

## LEDs

### Blink
```c++
// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(A0, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(A0, HIGH);  // turn the LED on (HIGH is the voltage level)
  delay(1000);                      // wait for a second
  digitalWrite(A0, LOW);   // turn the LED off by making the voltage LOW
  delay(1000);                      // wait for a second
}
```

#### Challenges
1. Make the pause between blinks shorter.
1. Blink Morse code for TVS (T is **-** V is **...-** S is **...**)
    - A - is 3 times as long a ., the space between letters is as long as a -
1. Google a Morse code chart and make it blink another message
1. Add a second LED and make them blink, but only one on at a time (when one is on, the other is off).

## Servos

### Sweep
```c++
#include <Servo.h>

Servo myservo;  // create servo object to control a servo

int pos = 0;    // variable to store the servo position

void setup() {
  myservo.attach(8);  // attaches the servo on pin 8 to the servo object
}

void loop() {
  for (pos = 0; pos <= 180; pos += 1) { // goes from 0 degrees to 180 degrees
    myservo.write(pos);              // tell servo to go to position in variable 'pos'
    delay(15);                       // waits 15 ms for the servo to reach the position
  }
  for (pos = 180; pos >= 0; pos -= 1) { // goes from 180 degrees to 0 degrees
    myservo.write(pos);              // tell servo to go to position in variable 'pos'
    delay(15);                       // waits 15 ms for the servo to reach the position
  }
}

```

#### Challenges
1. Make the servo go faster one direction than the other
2. Make the servo wait when it gets to the end of each part of its sweep
1. Add a second servo that goes in opposite directions
1. Add an LED or two that do things in a pattern with the servos.

## 3d Printing

Join our class on [TinkerCad](https://www.tinkercad.com/joinclass). The join code is YXFJXSX7R.