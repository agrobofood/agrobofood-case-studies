Open Source Navigation
======================

**SLAM algorithm**

SLAM stands for Simultaneous Localization and Mapping, which is a category 
of algorithms that has various implementations [44-46, 130]. All mobile 
robotic devices including (semi-) self-driving cars use this type of 
algorithm. For the current version of this document, it is unclear if 
there already is a best practice regarding the choice and implementation 
of SLAM for agriculture robotics. The natural yet repetitive environment 
makes it hard to use landmarks for map-building and navigation, yet (at 
least for outdoor agriculture) the GNSS is highly accurate.

**Path planning algorithm**

Path planning is a generic algorithm that will be present 
in all mobile robots [52]. In agriculture, path planning is in some regards
simpler than in challenging environments such as crowded public spaces. A 
difficult challenge remains the presence of foliage which should not be 
considered as a hard constraint, but can (and must) occasionally be pushed 
aside.

Recommendations
---------------

When implmenting navigation on mobile robots it is always a good choice to
start with the ROS/ROS2 navigation stack. It is one of the most used navi-
gation stacks in robotics and can be easily extended. 
Inputs generally required in Navigation Stack are odometry and sensor data
such as a continuous stream of 2D/3D scans or 3D point clouds of the 
immediate environment. Outputs are velocity commands sent to a mobile 
base.

Related Links & Literature
--------------------------
[1] https://navigation.ros.org/