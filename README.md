# Arduino Ultrasonic Sensor Projects

A practical collection of beginner-friendly Arduino projects using the HC-SR04 ultrasonic sensor.

The examples cover distance measurement, obstacle detection, smart dustbin projects, and basic robotics applications.

## Contents

- HC-SR04 basics
- Distance measurement
- Obstacle detection
- Smart dustbin
- Robotics applications
- Troubleshooting
- Useful resources

## HC-SR04 basics

The HC-SR04 measures distance by sending an ultrasonic pulse and timing how long it takes for the reflected signal to return.

Typical connections with an Arduino Uno:

| HC-SR04 pin | Arduino Uno |
|---|---|
| VCC | 5V |
| GND | GND |
| TRIG | D9 |
| ECHO | D10 |

A simplified distance calculation is:

`distance = time × speed_of_sound / 2`

The division by two accounts for the outgoing and returning sound wave.

## Distance measurement

The simplest project is to read the distance from the HC-SR04 and print the result to the Serial Monitor.

See [code/hc-sr04-distance.ino](code/hc-sr04-distance.ino).

## Obstacle detection

Once distance readings are reliable, the sensor can be used to detect nearby objects.

Common applications include:

- Obstacle-avoiding robots
- Parking assistance
- Automatic doors
- Presence detection
- Prototype automation systems

A project can set a threshold such as 20 cm and trigger an LED, buzzer, motor or servo when an object is detected closer than that value.

## Smart dustbin

A common beginner project combines an HC-SR04 ultrasonic sensor with a servo motor.

The sensor detects a hand near the lid and the Arduino commands the servo to open it. After a short delay, the lid can close again.

Typical components:

- Arduino Uno
- HC-SR04
- Servo motor
- Breadboard
- Jumper wires
- Power source

For a detailed walkthrough and additional project ideas, see the [Vayuyaan ultrasonic sensor projects guide](https://vayuyaan.com/blog/top-10-ultrasonic-sensor-projects-for-engineering-students/).

## Robotics applications

Ultrasonic sensors are useful in beginner robotics because they provide a simple way to estimate the distance to nearby obstacles.

A basic obstacle-avoiding robot can:

1. Measure the distance ahead.
2. Stop when an obstacle is too close.
3. Compare alternative directions.
4. Turn toward a clearer path.
5. Continue moving.

## Troubleshooting

### Readings are zero

Check power and ground connections first. Confirm that TRIG and ECHO are connected to the pins used by the code.

### Readings jump around

Avoid pointing the sensor at soft or sharply angled surfaces. Secure the wiring and take multiple readings when your application needs more stability.

### The sensor detects nothing

Make sure the object is within the useful operating range and that the ECHO pin is configured as an input.

## Useful resources

- [Vayuyaan ultrasonic sensor projects guide](https://vayuyaan.com/blog/top-10-ultrasonic-sensor-projects-for-engineering-students/)
- [Arduino documentation](https://docs.arduino.cc/)

## Contributing

Ideas, corrections and additional beginner-friendly projects are welcome.

## License

This project is licensed under the MIT License.
