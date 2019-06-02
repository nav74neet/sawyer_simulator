sawyer_simulator
================

Gazebo simulation with emulated interfaces for the Sawyer Robot (to be used with sawyer_gail repository).
This repository also installs the intera sdk & intera common tools and packages.

Installation:
-------------
Followed from <a href= "https://github.com/nav74neet/sawyer_robot">sawyer_robot</a> package setup
```
$ cd ~/sawyer_ws/src
$ git clone https://github.com/RethinkRobotics/sawyer_simulator.git
$ cd ~/sawyer_ws/src
$ wstool init .
$ wstool merge sawyer_simulator/sawyer_simulator.rosinstall
$ wstool update
```
Building from the source:
```
$ source /opt/ros/kinetic/setup.bash
$ cd ~/sawyer_ws/
$ catkin_make
```
Note:
-----
Copy the <b>intera.sh</b> file from the inter sdk folder to the ros_ws folder & change the ros_version to kinetic and edit the ip configuration and hostname. 

**To activate the sawyer workspace:**
```
$ cd sawyer_ws
$ ./intera.sh sim  
```
