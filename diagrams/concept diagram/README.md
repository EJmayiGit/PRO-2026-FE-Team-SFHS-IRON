# CONCEPT DIAGRAM
This diagram shows the initial system architecture of our robot, including sensor connections, motor configuration, and SPIKE Prime hub integration.

![image alt](https://github.com/EJmayiGit/PRO-2026-FE-Team-SFHS-IRON/blob/main/diagrams/concept%20diagram/Simple%20Concept-schematic.png?raw=true)

> The components shown in the CircuitCanvas diagram are used for conceptual representation. 
While some elements in the diagram may not exactly reflect the physical implementation, they are intended to represent the functional relationships within the system.

# COMPONENTS FUNCTION

# SPIKE Prime Hub
The SPIKE Prime Hub serves as the central controller of the system. It processes all sensor inputs, executes the control logic, and sends commands to the motors. 
In the concept diagram, the battery symbol represents the hub, indicating its role as both the control unit and power source.

# SPIKE Medium Motor
The SPIKE Medium Motor is positioned at the front and functions as the steering actuator. It controls the orientation of the front axle, enabling the robot to turn left or right. 
This configuration mimics a car-like steering mechanism rather than differential drive.

# SPIKE Large Motor
The SPIKE Large Motor is mounted at the rear of the robot and is responsible for propulsion. 
It provides forward and backward motion. Speed control of this motor directly determines the robot’s linear velocity.

# SPIKE Distance Sensors
The distance sensors are used to measure the distance between the robot and surrounding walls or obstacles. 
These measurements are used to:
* Maintain proper alignment within the track
* Support wall-following behavior

# SPIKE Color Sensors
The color sensors are used to detect colored obstacles on the track. These inputs determine navigation decisions, specifically differentiating obstacle types based on color and follow the game's mechanics.

# Built-in Gyro Sensor
The built-in gyro sensor of the SPIKE Prime Hub is used to measure the robot’s orientation and angular movement. 
It provides real-time feedback on the robot’s heading, allowing the control system to correct deviations during motion. This improves the accuracy of turns, stabilizes straight-line movement, and enhances overall navigation consistency.

# HOW IT OPERATES?
The robot operates by combining distance measurements from ultrasonic sensors and color detection from the color sensors. The control algorithm processes these inputs to determine steering adjustments via the front motor and propulsion control via the rear motor. In addition, the system utilizes the built-in gyro sensor of the SPIKE Prime Hub to maintain orientation and ensure smooth and stable navigation. This results in a reliable, sensor-driven system suitable for autonomous operation in the competition environment.
