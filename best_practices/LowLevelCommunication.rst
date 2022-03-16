Open Source Low-level Communication
===================================

CAN-bus has been adopted as ISO standard 11783 (also known as 
“ISOBUS”[34, 35]) for agriculture machinery. It should be used 
for the low-level communication between motion controllers, actuators,
and other components. Unfortunately, this conflicts with the internal 
low-level communication inside common mobile robotics platforms.

Common protocols used in robotics for low-level communication are EtherCAT
and CANopen. For both protocols there are open source libraries available in
order to communicate with low level devices.

Recommendations
---------------
Use ISOBUS when you develop low-level components for the agricultural
machinery market. If you are developing agricultural robot systems,
choose the communication protocol that is fit for your use case and
for which the necessary components are available. Avoid having multiple
bussystems in your robot. EtherCAT, CANopen and ISOBUS are prooven in use
for this application and for each bus an open source reference
implementation exists.

Related Links & Literature
--------------------------
[1] https://github.com/OpenEtherCATsociety/soem

[2] https://gitlab.com/etherlab.org/ethercat

[3] https://github.com/lely-industries/lely-core

[4] https://git.osb-connagtive.com/isobus/public/ISOAgLib
