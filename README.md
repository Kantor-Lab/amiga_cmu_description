# amiga_cmu_description
This a ROS robot description package for an amiga_robot urdf description
## Installation
Install the amiga_robot description

```
cd ~/catkin_ws/src
git clone -b ruiji https://github.com/Kantor-Lab/amiga_cmu_description.git
```
Install xarm_ros package (optional for current version)
```
cd ~/catkin_ws/src
git clone -b corn_insertion https://github.com/Kantor-Lab/xarm_ros.git
```
Update the package (optional for current version)
```
cd ~/catkin_ws/src/xarm_ros 
git pull
git submodule sync
git submodule update --init --remote
```
Go back to the catkin_ws and do catkin_make
```
cd ~/catkin_ws && catkin_make
```
## Test the package
First use this to source the environment
```
cd ~/catkin_ws 
source devel/setup.bash
```
Check the RVIZ
```
roslaunch amiga_cmu_description farm-ng.launch
```
Check the gazebo
```
roslaunch amiga_cmu_description amiga-gazebo.launch

