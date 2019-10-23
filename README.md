# How to install
This is made for WidowX in ros-melodic

Official Cite: https://github.com/Interbotix/widowx_arm

## Install prerequisites
```
sudo apt-get isntall build-essential libgtk-3-dev
sudo apt-get install ros-melodic-moveit ros-melodic-pcl-ros
```

## Clone widowx_arm_melodic repository and build
Go to your workspace
```
git clone https://github.com/Interbotix/widowx_arm.git
git clone https://github.com/Interbotix/arbotix_ros.git -b parallel_gripper
cd ..
catkin_make
```

# How to run
Go to your workspace

## Run in simulation
```
source devel/setup.bash
roslaunch widowx_arm_bringup arm_moveit.launch sim:=true sr300:=false
```

## Run in real robot
Plug in your robot, and make sure your USB port is available
```
source devel/setup.bash
roslaunch widowx_arm_bringup arm_moveit.launch sim:=true sr300:=false
```

