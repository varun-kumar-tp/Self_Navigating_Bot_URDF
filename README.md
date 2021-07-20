# Self-Navigating Bot URDF
The Universal Robot Description Format (URDF) is used for representing the robot model in ROS visualization tool (RViz). 

## Solidworks
Initially a 3D model of the bot is built in Solidworks. The following image shows the 3D model. 
![navigator in Gazebo](https://github.com/varunkumartp/Self_Navigating_Bot_URDF/blob/master/navigator_description/images/Solidworks.png)
The URDF of the model is extracted uing URDF_exporter pluggin for Solidworks.

## Prerequisites
Install the [ROS Noetic](http://wiki.ros.org/noetic/Installation/Ubuntu) framework for Ubuntu 20.04.

## Setup
### Create a workspace
``` bash
mkdir -p ~/project/src
cd ~/project/src
```
### Clone the git repository into the src folder
```bash
# Git must be installed
git clone https://github.com/varunkumartp/Self_Navigating_Bot_URDF
cd ..

# Build the code
catkin_make

# If no errors run
source devel/setup.bash
```

## Usage

### RViz
```bash
# open a terminals
cd ~/project

# source the terminal
source devel/setup.bash

# Command
roslaunch navigator_description display.launch
```

### Gazebo
```bash
# open a terminals
cd ~/project

# source the terminal
source devel/setup.bash

# Command
roslaunch navigator_bringup gazebo.launch
```
## Results

### Rviz
The following image shows the URDF model visualized in Rviz
![navigator in Rviz](https://github.com/varunkumartp/Self_Navigating_Bot_URDF/blob/master/navigator_description/images/rviz.png)

### Gazebo
The following image shows the URDF model visualized in Gazebo
![navigator in Gazebo](https://github.com/varunkumartp/Self_Navigating_Bot_URDF/blob/master/navigator_description/images/gazebo.png)
