
web_server
=====================================================================

This package contains the visulation of robot model and robot model controller in web server.

Dependencies
=====================================================================
[The MoveIt! smart wrist package](https://github.com/fontyssmartwrist/moveit_smart_wrist)

[The robot model](https://github.com/fontyssmartwrist/sw_v3_description)

[The MoveIt! commander ROS node](https://github.com/fontyssmartwrist/smart_movement)

Install guide
=====================================================================
   1) Install MoveIt! kinetic with the following command

	sudo apt install ros-kinetic-moveit

   2) Install MoveIt! TRAC-IK plugin with the following command

	sudo apt-get install ros-kinetic-trac-ik-kinematics-plugin
   
   3) Install rosbridge server with the following command
   
    sudo apt-get install ros-kinetic-rosbridge-server
   
   4) Clone this project and the dependencies to your catkin's workspace src folder
   5) Run catkin_make to build 

Running
=====================================================================
Start with running the MoveIt! package launch file with the following command in the terminal
    
    roslaunch moveit_smart_wrist demo.launch
   
To start the web server:
    
    roslaunch web_server webserver.launch
    
To start the commander node:
   
    rosrun smart_movement web_moveit_coordinate_node.py
 
Documentation
=====================================================================
Documentation how it works can be found in 

Documentation_on_MoveIt.pdf 
https://github.com/fontyssmartwrist/smart_movement/blob/master/Documentation_on_MoveIt.pdf  

Web_ROS_CodeSys_Report.pdf
https://github.com/fontyssmartwrist/web_server/blob/master/Web_ROS_CodeSys_Report.pdf

Authors
=====================================================================
Aike van Alkemade

Zhicheng Yu
