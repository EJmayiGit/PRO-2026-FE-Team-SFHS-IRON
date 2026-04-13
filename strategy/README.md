# TEAM STRATEGIES
This folder presents the complete navigation strategy of our robot for both the Open Challenge and Obstacle Challenge in the 25th PRO Future Engineers competition.
The strategies shown here are designed to ensure consistent and stable performance despite random changes in the track layout.

# Open Challenge
In the Open Challenge, the layout of the track changes every round, particularly the placement and spacing of the interior walls. Because of this, the robot cannot rely on fixed paths and must instead adapt dynamically using sensor feedback.
Our strategy is based on **wall-referenced navigation combined with gyro stabilization**.

To maintain a consistent path, our robot uses a side-mounted ultrasonic sensor to measure the distance from the inner wall. 
This allows the robot to follow the wall and keep a roughly parallel trajectory throughout straight sections. 
Instead of relying on a single reading, the robot continuously monitors the distance and applies small steering corrections to maintain stability.

