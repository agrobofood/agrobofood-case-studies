Open Source Manipulation
========================


Once the location and orientation of the crop has been determined, 
the robot must decide how to position the end effector. This is a 
constrained optimization problem where the stem should be cut but no 
other plant parts should be damaged.

While weeding end-effectors can usually move in a straight line toward 
the weed, for crop harvesting there are often severe obstacles such 
as branches and other unripe or un(der)developed crops. This 
requires advanced path planning algorithms to avoid those obstacles. 
The current best practice is to use a randomized or optimizing motion 
planner as implemented in OMPL which can be used through the package 
MoveIt in ROS. New motion planning algorithms are still in development, 
and a very interesting research avenue is to plan motions that purposefully 
push parts of the obstacles away. Retrieving the crop is yet another 
challenging motion planning problem, because now a collision-free motion 
for the manipulator including the crop must be found.

Recommendations
---------------
MoveIt is a user-friendly open-source robotics manipulation platform 
which runs on top of ROS and ROS2. It leverages ROS software by providing
high-level functionalities for robotics manipulation such as collision
checking, inverse kinematic algorithms, trajectory processing, etc. 
To the best of our knowledge, it is one of the most widely used open-source
robotics manipulation platforms for developing commercial applications, 
prototyping designs, and benchmarking algorithms. 

If you are looking for a solution without using MoveIt, there is an alternative
motion planning software called tesseract_ros.

If you do not want to use ROS and MoveIt you can use OMPL, which provides
a large number of advanced manipulation algorithms.


Related Links & Literature
--------------------------
[1] https://moveit.ros.org/

[2] https://github.com/tesseract-robotics/tesseract_ros

[3] https://ompl.kavrakilab.org/
