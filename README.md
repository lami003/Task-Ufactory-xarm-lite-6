Task-Ufactory-xarm-lite-6

Ufactory XArm Lite 6 — ROS 2 URDF Package

 Overview

This ROS 2 package provides the URDF (Unified Robot Description Format) model for the Ufactory XArm Lite 6 robotic arm.
It includes all links, joints, and 3D meshes required to visualize and simulate the robot in tools such as RViz2.


 Prerequisites

Before using this package, ensure you have the following installed:

ROS 2 (any supported distribution)

colcon build tool

rviz2 (for visualization)

Git (for cloning the repository)

 
1. Clone the repository
git clone https://github.com/lami003/Task-Ufactory-xarm-lite-6.git

2. Build the package
cd ~/ros2_ws
colcon build

3. Source the workspace
source install/setup.bash

 Visualize in RViz2

You can launch and visualize the robot using the URDF model with the following command:

ros2 launch urdf_tutorial display.launch.py model:=$PWD/arm_description/urdf/arm.urdf

 Notes

Ensure that all mesh files are located in the meshes/ directory and referenced correctly in the URDF.

The package structure follows standard ROS 2 conventions for robot description packages.
