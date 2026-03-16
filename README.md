# Arduino Line Follower Robot

This project is a simple line follower robot built using Arduino.  
The robot is able to follow a black line drawn on a white surface.  
It uses two IR sensors to detect the line and adjusts the motors so that it stays on the path.

I built this project to understand how sensors, motor drivers and basic control logic work together in a small robotics system.

## Components Used

- Arduino Uno  
- L298N Motor Driver  
- 2 IR Sensors  
- 2 DC Motors  
- Robot Chassis  
- Battery Pack  
- Connecting Wires  

## How the Robot Works

Two IR sensors are placed at the front of the robot, one on the left and one on the right.  
These sensors check the surface below them and send signals to the Arduino.

Based on the sensor readings, the Arduino decides how the motors should move.

| Left Sensor | Right Sensor | Robot Action |
|-------------|-------------|--------------|
| LOW | LOW | Move Forward |
| LOW | HIGH | Turn Left |
| HIGH | LOW | Turn Right |
| HIGH | HIGH | Stop |

This simple logic allows the robot to continuously adjust its direction and stay on the line.

## What I Learned

While building this project I learned:

- how IR sensors detect different surfaces  
- how to control DC motors using the L298N motor driver  
- how to write Arduino logic to control a robot’s movement  
- how simple sensor feedback can be used to guide a robot

## Possible Improvements

Some things that could be added in the future:

- using more sensors for better accuracy  
- implementing PID control for smoother motion  
- increasing speed while maintaining stability
