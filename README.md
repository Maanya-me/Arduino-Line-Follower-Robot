Overview:  
This project is a simple Arduino-based line follower robot. The robot is able to detect a black line on the floor and follow it automatically. It uses two IR sensors to sense the line and control the direction of the motors so that the robot stays on the path.

Features:

1. Line Following: Uses two IR sensors placed at the front of the robot to detect the black line.
2. Direction Control: The robot adjusts the direction of the motors depending on which sensor detects the line.
3. Simple Logic Control: The movement is controlled using basic Arduino logic based on sensor readings.
4. Modular Code: The code is written in simple functions for motor control and sensor reading.

Components:

1. Arduino Uno  
2. L298N Motor Driver  
3. DC Motors (2)  
4. IR Sensors (2)  
5. Robot Chassis  
6. Battery Pack  
7. Connecting Wires  

Circuit Diagram:

The IR sensors are connected to the digital input pins of the Arduino to read line detection signals.  
The L298N motor driver is connected to the Arduino output pins to control the direction and speed of the DC motors.

Code Explanation:

1. setup(): Initializes the motor driver pins and IR sensor pins and prepares the robot to start moving.

2. loop(): Continuously reads the values from the left and right IR sensors and decides how the robot should move.

3. rotateMotor(): Controls the direction of the motors based on the speed values provided by the main logic.

4. Motor Logic:  
   - If both sensors detect white surface → robot moves forward  
   - If the left sensor detects the line → robot turns left  
   - If the right sensor detects the line → robot turns right  
   - If both sensors detect the line → robot stops
