# Arduino Line Follower Robot

This is a small robot made using Arduino that can follow a black line on the floor.  
The idea is simple: the robot uses two IR sensors to check the surface below it and moves according to what the sensors detect.

## Components Used

- Arduino Uno
- L298N Motor Driver
- 2 IR Sensors
- 2 DC Motors
- Robot Chassis
- Battery Pack
- Connecting Wires

## How the Robot Works

Two IR sensors are placed at the front of the robot.  
These sensors check whether the surface below them is black or white.

If both sensors see white, the robot moves forward.  
If one sensor sees the black line, the robot turns in that direction to stay on the path.  
If both sensors detect the line, the robot stops.

## What I Learned

While building this project I learned:
- how to read sensor values using Arduino
- how to control DC motors using a motor driver
- how simple logic can be used to control a robot's movement
