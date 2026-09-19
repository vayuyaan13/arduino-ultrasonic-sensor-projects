# HC-SR04 Distance Measurement with Arduino

Measure the distance between an HC-SR04 ultrasonic sensor and an object with an Arduino Uno.

## Components

- Arduino Uno
- HC-SR04 ultrasonic sensor
- Breadboard
- Jumper wires

## Wiring

| HC-SR04 | Arduino Uno |
|---|---|
| VCC | 5V |
| GND | GND |
| TRIG | D9 |
| ECHO | D10 |

## How it works

The Arduino sends a short trigger pulse. The HC-SR04 emits an ultrasonic burst and raises its ECHO output for the travel time of the reflected signal.

The code converts that time into centimeters using the approximate speed of sound in air.

See [the example sketch](../code/hc-sr04-distance.ino).
