# Arduino Line Follower Robot

This project implements a simple **Line Follower Robot using Arduino** and **IR sensors**.  
The robot detects a black line on a white surface and automatically follows the path by controlling two DC motors.

## Components Used

- Arduino Uno
- L298N Motor Driver
- 2 IR Sensors
- 2 DC Motors
- Robot Chassis
- Battery Pack
- Connecting Wires

## Working Principle

The robot uses two IR sensors placed on the left and right side.

| Left Sensor | Right Sensor | Action |
|-------------|-------------|------|
| LOW | LOW | Move Straight |
| LOW | HIGH | Turn Left |
| HIGH | LOW | Turn Right |
| HIGH | HIGH | Stop |

The Arduino reads sensor values and adjusts motor direction and speed accordingly.

## Features

- Real-time line detection
- Differential motor control
- Adjustable motor speed using PWM

## Applications

- Autonomous robots
- Warehouse robots
- Path following automation

## Author

Maanya  
B.Tech Engineering Physics  
IIT Ropar
