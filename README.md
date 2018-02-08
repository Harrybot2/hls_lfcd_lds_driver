# hls_lfcd_lds_driver

ROS package for HLDS HLS-LFCD LDS driver

ROS Wiki: [hls_lfcd_lds_driver](http://wiki.ros.org/hls_lfcd_lds_driver)

ROS Packages Maintainer: [ROBOTIS](http://wiki.ros.org/ROBOTIS)

Manufacturer of the LDS: [Hitachi-LG Data Storage](http://hlds.co.kr/v2/e_index.html)

Reseller of the LDS:[Fidurobot](http://www.fidurobot.com)

# Overview

The hls_lfcd_lds_driver package is a driver for HLS(Hitachi-LG Sensor) LFCD LDS(Laser Distance Sensor). The LDS is a sensor sending the data to Host for the simultaneous localization and mapping (SLAM). Simultaneously the detecting obstacle data can also be sent to Host. HLDS(Hitachi-LG Data Storage) is developing the technology for the moving platform sensor such as Robot Vacuum Cleaners, Home Robot, Robotics Lawn Mower Sensor, etc.

![HLS-LFCD2](http://wiki.ros.org/hls_lfcd_lds_driver?action=AttachFile&do=get&target=LDS.png)


# User's Guide

## Install
```
sudo apt-get install ros-kinetic-hls-lfcd-lds-driver
```
or download the driver into your catkin_**/src，and compile it.

## Setting the permissions of HLS-LFCD2
connect the lidar with your computer,and run below:
```
sudo chmod a+rw /dev/ttyUSB0
```

## Run hlds_laser_publisher node
run ros:
roscore
Open another terminal,

```
source devel/setup.bash
roslaunch hls_lfcd_lds_driver hlds_laser.launch
```

## Run hlds_laser_publisher node with RViz
Open another terminal,

```
source devel/setup.bash
```
roslaunch hls_lfcd_lds_driver view_hlds_laser.launch
```

# Report a Bug

* [List Active Tickets](https://github.com/ROBOTIS-GIT/hls_lfcd_lds_driver/issues)

* [Open a New Ticket](https://github.com/ROBOTIS-GIT/hls_lfcd_lds_driver/issues/new)
