Open Source Field Busses
=========================

When developing an agricultural robot, it is often necessary to connect equipment such as grippers, sensors or other actuators. 
This is usually done using a field bus. While ISOBUS is the standard in large agricultural machinery, in robotics CANopen and
EtherCAT are predominant due to their good support of motion control. For all three field busses open source libraries exist.
For EtherCAT and CANopen there are integrations into the Robot Operating System.

Recommendations
---------------
We therefore recommend the following best practices:
* For interfaces that are not interfacing with agricultural machinery use CANopen or EtherCAT
* For interfaces that are interfacing with agricultural machinery use ISOBUS
* For interfaces that require high frequency motion control (>100Hz) use EhterCAT
