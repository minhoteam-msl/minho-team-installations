#ROS Installation Guide

$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

$ sudo apt-key adv --keyserver hkp://ha.pool.sks-keyservers.net:80 --recv-key 0xB01FA116

$ sudo apt-get update

$ sudo apt-get install ros-kinetic-desktop

$ sudo rosdep init

$ rosdep update

$ echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc

$ source ~/.bashrc

$ source /opt/ros/kinetic/setup.bash

$ cd ~

$ mkdir catkin_ws

$ cd catkin_ws

$ mkdir src

$ cd src

$ catkin_init_workspace

$ cd ~/catkin_ws

$ catkin_make

$ echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc

$ sudo apt-get -y install libcgal-*
