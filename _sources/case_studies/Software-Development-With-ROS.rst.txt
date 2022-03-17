Development of a ROS2 component
===============================

When you are developing a ROS2 system usually you will first check if
the ROS2 ecosystem does not provide all components that you need for your
system. If components are missing, you need to develop the component on your
own. In this case study we will take a look into the steps necessary for
such a development.

1. Planning & Design
---------------------
Before starting with the development of your ROS2 package, you need to plan
a few things. Most importantly, you should already decide whether your
package will be open sourced and if so which **open source license** to use for your package. 
Also if you want to integrate your ROS2 package into a ROS Distro you
need to think about how you want to maintain the package and what kind of
quality level your package should have. **ROS2 package quality levels** can be
acessed here: https://discourse.ros.org/t/rep-2004-package-quality-categories/11988
Another choice you should take right at the beginning, is which programming
language you want to use for your ROS2 package. Prime support in ROS2 exists
for C, C++ and Python, but other languages can also be used.

2. Workspace Setup & Package Creation
-------------------------------------
Once the initial decisions are done you can start creating your development
workspace and packages. ROS2 documentation provides excellent tutorials for
this.


3. Development Environment
-------------------------------
You can use any IDE of your choice to program ROS2 packages. However,
Visual Studio Code currently provides quite extensive support for  
ROS and also extension packages for Python, C and C++, as well as CMAKE
via Extensions.

4. Version Control System
--------------------------
Once you setup your package, workspace and IDE, it is time to think about
the version control system you want to use. For ROS the only
sensible choice is using GIT as version control system. You are free in
choice of the hoster, but most ROS apckages are hosted on GitHub.


5. Continuous Integration
-------------------------
Before you really start coding it also makes sense to setup your continuous
integration system already.



