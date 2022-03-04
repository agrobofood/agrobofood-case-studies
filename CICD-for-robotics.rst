Continuous Integration for Robotics
===================================


Popular CI/CD tools
-------------------

GitHub actions
"""""""""""""""
GitHub Actions makes it easy to automate all your software workflows, now with world-class CI/CD. Build, test, 
and deploy your code right from GitHub. Make code reviews, branch management, and issue triaging work the way you want.

GitLab CI 
"""""""""""""
GitLab CI/CD is a tool for software development using the continuous methodologies such as Continuous Integration (CI),
Continuous Delivery (CD), Continuous Deployment (CD). Use GitLab CI/CD to catch bugs and errors early in the development
cycle. Ensure that all the code deployed to production complies with the code standards you established for your app.
GitLab CI/CD can automatically build, test, deploy, and monitor your applications by using Auto DevOps.
For a complete overview of these methodologies and GitLab CI/CD, read the Introduction to CI/CD with GitLab.

Travis 
"""""""""""""
Travis CI is a hosted continuous integration service used to build and test software projects hosted on GitHub and Bitbucket.
Travis CI was the first CI service which provided services to open-source projects for free and continues to do so. TravisPro
provides custom deployments of a proprietary version on the customer's own hardware.
The source is technically free software and available piecemeal on GitHub under permissive licenses. 
The company notes, however, that the large number of tasks that a user needs to monitor and perform can
make it difficult for some users to successfully integrate the Enterprise version with their own infrastructure.

Jenkins 
"""""""""""""
Jenkins is an open source automation server. It helps automate the parts of software development related to building, testing,
and deploying, facilitating continuous integration and continuous delivery. It is a server-based system that runs in servlet
containers such as Apache Tomcat. It supports version control tools, including AccuRev, CVS, Subversion, Git, Mercurial, Perforce,
ClearCase and RTC, and can execute Apache Ant, Apache Maven and sbt based projects as well as arbitrary shell scripts and Windows
batch commands.

BuildBot 
"""""""""""""
Buildbot is a software development continuous integration tool which automates the compile or test cycle required to validate 
changes to the project code base. It began as a light-weight alternative to the Mozilla project's Tinderbox, and is now 
used by Python, WebKit, LLVM, Blender, ReactOS and many other projects.


Open source robotics tools
--------------------------
In robotics a number of open source tools exist that simplify continuous integration for robotics
software. 

industrial_ci
"""""""""""""
industrial_ci is a tool that simplifies continuous integration tasks for repositories containing
ROS packages. It enables building ROS packages, checking compatibility with different ROS distributions,
running unit and integration tests, linting checks and much more. Another advantage is that it can be
used with different CI/CD systems (GitHub Actions, GitLab CI, Travis and others). It supports ROS1
and ROS2.


action-ros-ci
"""""""""""""
action-ros-ci is a GitHub action for enabling continuous integration for repositories containing ROS packages
on GitHub actions only. It enables building ROS, checking compatibility with different ROS distributions,
running unit and integration tests, linting checks and much more. 

Best practices
---------------
The popular CI tools all have their reasons to exist. In order to give some guidance which tool
is best for which application, we make recommendations for open source projects and closed source
projects seperately. Where closed source projects are all projects that are not released under
open source license and hosted on public platforms.

Open Source Robotics Projects
"""""""""""""""""""""""""""""
* Host project repository on github.com, use Github Actions and either industrial_ci or action-ros-ci.
* Host project on Bitbucket and use Travis CI with industrial_ci
* Host project on GitLab.com and use industrial_ci


Closed Source Robotics Projects
"""""""""""""""""""""""""""""""
* Host project on premise GitLab instance, use Gitlab CI and industrial_ci
* Host your project on premise and use BuildBot or Jenkins