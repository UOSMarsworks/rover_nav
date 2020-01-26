# rover_nav

## Requirements
### System requirements
* Ubuntu 16.04
* ROS kinect
* Gazebo 7 (needed for running simulations only)

### ROS packages
* realsense2_camera
  * Install from  [here](https://github.com/IntelRealSense/realsense-ros).
* elevation_mapping
  * Install from [here](https://github.com/ANYbotics/elevation_mapping).
* ocotmap
```shell
sudo apt install ros-kinetic-octomap
sudo apt install ros-kinetic-octomap-server
```

## Installation
```bash
sudo apt-get update
sudo apt-get upgrade
cd catkin_ws/src
git clone https://gitlab.com/marsworks/rover_nav
git clone https://gitlab.com/marsworks/rover_description
git clone https://github.com/ros-planning/navigation.git
cd ..
catkin_make
source devel/setup.bash
```

## Usage Instructions
* Octomap + 2D navigation + simultaion
```bash
roslaunch rover_nav sim_2D_nav.launch
```
* Octomap + 2D navigation + hardware
```bash
roslaunch rover_nav hardware_2D_nav.launch
```
