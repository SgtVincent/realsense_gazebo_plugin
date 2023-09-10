# Intel RealSense Gazebo ROS plugin

This package is a Gazebo ROS plugin for the Intel D435 realsense camera, tested on ROS Noetic and Gazebo 11. 
 
## Acknowledgement

This package is forked from [realsense_gazebo_plugin](https://github.com/pal-robotics/realsense_gazebo_plugin) and integrates the urdf/ launch files from [realsense-ros-gazebo](https://github.com/rickstaa/realsense-ros-gazebo) and fix from 


## Installation

You should have ROS Noetic, gazebo_ros (Gazebo 11), and realsense ROS packages already installed. For example, with [Robostack](https://robostack.github.io/index.html) a ROS environment integrated with Conda, you can install the dependencies with:

```bash
# Install gazebo_ros_pkgs
mamba install ros-noetic-gazebo-ros ros-noetic-gazebo-ros-pkgs

# Install realsense ROS packages
mamba install ros-noetic-realsense2-camera ros-noetic-realsense2-description ros-noetic-librealsense2
```

Then, clone this repository into your catkin workspace and build it with `catkin build`:

```bash
cd /path/to/catkin_ws/src
git clone git@github.com:SgtVincent/realsense_gazebo_plugin.git
cd ..
catkin build realsense_gazebo_plugin
```

## Usage

There are example lauch files in the `launch` folder. You can run them with:

```bash
source devel/setup.bash
roslaunch realsense_gazebo_plugin view_d435_model_rviz_gazebo.launch 
```
