# ROS REALITY

Hi, and welcome to ROS Reality, a virtual reality teleoperation interface for ROS enabled robots (we use a Baxter, but the code could easily be modified for any ROS robot). This readme contains all the information you need to get started.

## Overview

This package connects a ROS network to a remote windows machine running Unity, and uses sensor data sent on ROS topics to populate a virtual reality scene. The sensors we use are a Kinect v2, the wrist cameras of the robot, and the joint encoders of the robot.

## Dependencies

For this tutorial, we will focus on controlling a Baxter robot. Therefore you will need to install the Baxter SDK on you computer. You can find instructions for that here: http://sdk.rethinkrobotics.com/wiki/Workstation_Setup

To connect the Kinect to the ROS network, we use IAI Kinect, a ROS package found here: https://github.com/code-iai/iai_kinect2

To calibrate the Kinect, we use this package: https://github.com/ShibataLabPrivate/kinect_baxter_calibration

Finally, you will need to install rosbridge. You can install it via apt-get ```sudo apt-get install ros-indigo-rosbridge-suite```

## Running ROS Reality

To start ROS Reality, simply run the following command on your Baxter workstation:

``roslaunch ros_reality_bridge ros_reality_bridge.launch``

Great, now this computer is sending information about the ROS network. Go to your Unity computer and follow the intstructions here: https://github.com/h2r/ROS_reality

