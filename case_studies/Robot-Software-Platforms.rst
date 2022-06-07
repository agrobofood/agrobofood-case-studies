Robot Software Platforms
========================

Use Case
--------
Robotics is becoming more and more complex. When developing a new robot or application, writing all software for the robot and
integrating the software is becoming a more and more complex endeavour. Consequently, it is very difficult today to integrate self
written and third party software in a consistent way for use in product. A solution to this problem is using a robot software platform
that provides ready-to-use and compatible components for creating robots.


Approach
-------------------
Existing and most used open source robot software platforms were identified.

Robot Operating System (ROS)
""""""""""""""""""""""""""""
The Robot Operating System is probably the best known open source software development kit for robotics. 
It is proven in use and already in many robot products. Today, more than 80k developers (Kolak et al. 2020) 
have used ROS for building software on Github.

Robot Operating System 2 (ROS2)
"""""""""""""""""""""""""""""""
ROS also has a second version, that is being developed by major companies (https://docs.ros.org/en/rolling/Governance.html) 
and is cut towards industrial usage. The first stable release is from June 2020 and the package ecosystem is growing. 
It supports real-time and security requirements as well as functionality requirements modern robot software requires.

Yet another robot platform (YARP)
"""""""""""""""""""""""""""""""""
YARP supports building a robot control system as a collection of programs communicating in a peer-to-peer way, with an extensible
family of connection types (tcp, udp, multicast, local, MPI, mjpg-over-http, XML/RPC, tcpros) that can be swapped in and out
to match your needs.

The Robot Construction Kit (ROCK)
"""""""""""""""""""""""""""""""""
Rock is a software framework for the development of robotic systems. The underlying component model is based on the Orocos RTT
(Real Time Toolkit). Rock provides all the tools required to set up and run high-performance and reliable robotic systems for 
wide variety of applications in research and industry. It contains a rich collection of ready to use drivers and modules for 
use in your own system, and can easily be extended by adding new components.

Open Robot Control Software (OROCOS)
""""""""""""""""""""""""""""""""""""
Orocos is a portable C++ libraries for advanced machine and robot control. Over the years, Orocos has become a large project 
of middleware and tooling for development of robotics software. The main parts of this project are the Real Time Toolchain (RTT)
and the Orocos Component Library (OCL).

Other platforms
---------------
An extensive literature research has been conducted to identify other robot software platforms, that could be interesting to 
use in agricultural robots. Important characteristics such as activity status, package management support (important for ecosystem)
and model-driven development support (important for high quality software development) have been evaluated.


.. csv-table:: Platforms (last checked spring 2021)
   :header: "Name", "Publication", "Status", "PM", "MBD", "OSS"
   :width: 400 px

    GenoM, (Fleury et al. 1997; Mallet et al. 052010), Stale, No, Yes, No
    Smartsoft, (Schlegel et al. 1999), Active, No, Yes, Yes
    Orocos, (H. Bruyninckx 2002), Active, Partial*, No, Yes
    CoolBot, (Dominguez-Brito et al. 2004), Stale, No, , 
    Rock, (Rock 2008), Active, Partial*, No, Yes
    ROS, (Quigley et al. 2009), Active, Yes, Yes, Yes
    ESROCOS, (M. Arancon et al. 2017), Active, Possible*, No, Yes
    MARIE, (Cote et al. 2004), Stale, , , 
    ArmarX, (Vahrenkamp et al. 2015), Active, No, No, Yes
    YARP, (Metta et al. 2006), Active, Possible, No, Yes
    XBotCore, (Muratore et al. 42017), ?, No, , 
    RoboFrame, (S. Petters et al. 2007), Stale, No, , 
    Fawkes, (Niemueller et al. 2010), Active, No, No, Yes
    OpenRDK, (Calisi et al. 92008), Stale, No, , 
    RT-Middleware, (Ando et al. 2005), Active, Yes, Yes, Yes
    Orca, (Brooks et al. 2005), Stale, No, No, 
    RSCA, (Yoo et al. 102006), Stale, No, No, 
    PEIS, (M. Broxvall et al. 2007), Stale, , ,
    ASEBA, (Magnenat et al. 2007), Stale, , , 
    ORiN, (Mizukawa et al. 2002), Stale, , ,
    Player/Stage, (Brian P. Gerkey et al. 2003), Stale, , ,
    CAMUS, (Kim et al. 2005), Stale, Stale, , ,
    \-, (Kuo et al. 2005), Stale, , ,
    CLARAty, (Nesnas et al. 2003), Stale, , ,
    ACRoSeT, (Iborra et al. 2009), Stale, , ,
    RSB, (Wienke et al. 122011), Stale, , ,
    Rapyuta, (Hunziker et al. 052013), Active, , , No
    BIP, (Basu et al. 2011), Stale, , , 
    MiRo, (Utz et al. 2002), Stale, , ,
    AEROSTACK, (Sanchez-Lopez et al. 62016), Stale, , ,
    OCP, (Paunicka et al. 2001), Stale, , , 
    MOOS, (Benjamin et al. 2010), Stale, , ,
    OPRos, (Han et al. 2012), Stale, , ,


Lessons Learned
---------------
ROS, ROS2, YARP, ROCK and OROCOS are currently the most predominant open-source robot software frameworks. 
Concerning technical capabilities (more details in D1.14), all of these platforms enable building working 
robots and all have been deployed in real applications. That being said, ROS and ROS2 stand out concerning 
ecosystem size (>200.000 packages on GitHub and more than 80.000 developers (Kolak et al. 2020)) and 
governance (Technical steering committee with ~20 industrial companies). ROS/ROS2 is also the most 
commercially used open source software platform in robotics, notable examples are Locus Robotics, 
Fetch Robotics, Clearpath Robotics, PalRobotics, Robotnik and others. Most other platforms offer some kind 
of bridge into the ROS ecosystem. From a standardization viewpoint, we therefore recommend using ROS or 
ROS2 if a robot software platform is needed.


