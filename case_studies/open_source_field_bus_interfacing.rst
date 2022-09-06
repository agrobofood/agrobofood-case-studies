Interfacing with field busses using ROS2
=========================================

Use Case
---------
When developing an agricultural robot, it is often necessary to connect equipment such as grippers, sensors or other actuators. This is usually done
using a field bus. While ISOBUS is the standard in large agricultural machinery, in robotics other field busses are predominant.

Approach
--------
To decide which fieldbus to use in a robot we have made an analysis of available open source fieldbus implementations.

* **CANopen**:
  CANopen is a fieldbus which is based on the CAN bus that is widely used in service robotics and mobile devices.
  Its main purppose in such devices is usually the connection of the drive system. CANopen comes with standard profiles
  for a large range of devices (most important is probably the cia402 profile for motion controllers).
  Due to its predominance in service robotics, a high quality ros driver exists for ROS1 and a ROS2 driver is under
  development.
  
* **EtherCAT**:
  EtherCAT is a fielbus that is based on the Ethernet physical layer but implements a realtime protocol on top of it.
  This bus is also often used in robotics, mainly in industrial robotics in order to control drives, sensors and other
  systems. EhterCAT also has a safety extension called FSOE.
  A free and open source ROS1 and ROS2 driver exists.
  
* **ISOBUS**:
  ISOBUS is a fieldbus that is based on the CAN bus. It is widely used in large agricultural machinery. There it is often
  used for interfacing with agricultural equipment. An open source implementation exists called isoaglib (https://git.osb-connagtive.com/isobus/public/ISOAgLib)




Lessons learned
----------------
In robotics, CANopen and EtherCAT are predominantly used. There is not a lot of information
available about ISOSBUS in the robotics community and no ROS drivers exist. In our experience,
the following guidelines make sense:

* If you build a robot that does not need to interface with any agricultural external equipement, use CANopen or EtherCAT for your drivetrain
* If you build a robot that does need to interface with external agricultural equipment, use CANopen.
* If you build a robot that does need to support high frequency motion control (i.e. >100hz) use EtherCAT.
