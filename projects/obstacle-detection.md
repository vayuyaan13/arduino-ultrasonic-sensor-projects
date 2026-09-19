# Obstacle Detection with HC-SR04 and Arduino

An HC-SR04 can provide a distance estimate that an Arduino uses as a simple obstacle detector.

## Basic logic

1. Trigger the sensor.
2. Read the echo time.
3. Convert the time to distance.
4. Compare the distance with a threshold.
5. Trigger an output such as an LED, buzzer, motor or servo.

For example:

`distance < 20 cm` -> obstacle detected

`distance >= 20 cm` -> path appears clear

The correct threshold depends on the project, robot speed, sensor placement and environment.
