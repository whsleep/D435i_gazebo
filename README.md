# Intel RealSense Gazebo ROS plugin

This package is a Gazebo ROS plugin for the Intel D435i realsense camera. Through this package, one can run the D435i camera (in simulation) with a urdf/xacro files included within a launch flile.

This package has been developed and tested in ROS Noetic, Ubuntu 20.04.
## Demo
![Demo](https://github.com/whsleep/D435i_gazebo/blob/master/gif/demo.gif)

## [D435i actual params](https://www.intel.cn/content/www/cn/zh/products/sku/190004/intel-realsense-depth-camera-d435i/specifications.html)
# Before running
Firstly, you need to add the model file for Gazebo. 

Here are two links to choose the appropriate one for download.

[Link1](https://github.com/osrf/gazebo_models)

[Link2](https://download.csdn.net/download/allenhsu6/15382137)

After extracting the file, overwrite it in `~/your_gazebo_path/gazebo/models`.

# How to RUN:
## Create directory
```shell
mkdir catkin_ws
cd catkin_ws
mkdir src
cd src
```
## Clone code
```shell
git clone https://github.com/whsleep/D435i_gazebo.git
```
## Build
```shell
catkin_make
```
## Run
```shell
roslaunch d435i_gazebo D435i_test.launch
```
## Acknowledgement

This is a continuation of work done by [SyrianSpock](https://github.com/SyrianSpock) for a Gazebo ROS plugin with RS200 camera.

This package also includes the work developed by Intel Corporation with the ROS model fo the [D435](https://github.com/intel-ros/realsense) camera.

Finally this package is also  dependent on the work done by [Pal-Robotics](https://github.com/pal-robotics/realsense_gazebo_plugin).

# d435i_gazebo
