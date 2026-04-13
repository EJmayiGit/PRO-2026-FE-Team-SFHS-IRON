# OUR STRATEGIES
====
This folder presents the complete navigation strategy of our robot for both the Open Challenge and Obstacle Challenge in the 25th PRO Future Engineers competition.
The strategies shown here are designed to ensure consistent and stable performance despite random changes in the track layout.

# Open Challenge
In the Open Challenge, the layout of the track changes every round, particularly the placement and spacing of the interior walls. Because of this, the robot cannot rely on fixed paths and must instead adapt dynamically using sensor feedback.
Our strategy is based on **wall-referenced navigation combined with gyro stabilization**.

| Default Movement | Turning Mechanic |
| ---------------- | ---------------- |
| ![image](https://drive.google.com/file/d/1r9mGaHEz4q5lqStaKcmmNDQMkdPdIxoY/view?usp=sharing) | ![image](https://drive.google.com/file/d/1rKcfQgtBB3DHPeiyQU9a7iYfcC6d7Pey/view?usp=sharing) |

To maintain a consistent path, our robot uses a side-mounted SPIKE distance sensor to measure the distance from the inner wall. 
This allows the robot to follow the wall and keep a roughly parallel trajectory throughout straight sections. 
Instead of relying on a single reading, the robot continuously monitors the distance and applies small steering corrections to maintain stability. To ensure accurate and smooth movement, the robot utilizes the built-in gyro sensor of the SPIKE Prime hub

The robot determines when to turn by detecting the absence of a wall using the SPIKE distance sensor. When the measured distance suddenly increases beyond a defined threshold, the robot identifies this as an opening or corner. To improve reliability, this condition is confirmed over multiple readings before initiating a turn.

By combining ultrasonic sensing for environmental awareness and gyro feedback for motion control, the robot achieves a stable and adaptable navigation system capable of completing multiple laps consistently despite changes in the field layout.

