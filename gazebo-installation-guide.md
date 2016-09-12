#Gazebo Installation Guide

$ sudo sh -c 'echo "deb http://packages.osrfoundation.org/gazebo/ubuntu-stable `lsb_release -cs` main" > /etc/apt/sources.list.d/gazebo-stable.list'

$ wget http://packages.osrfoundation.org/gazebo.key -O - | sudo apt-key add -

$ sudo apt-get update

$ sudo apt-get install libgazebo7-dev

$ sudo apt-get install ros-kinetic-gazebo-ros-pkgs

#### Install SDF

[Download source files in http://sdformat.org/download]
[Extract to ~]

$ cd ~/sdf-[VERSION]

$ mkdir build

$ cd build

$ cmake ..

$ make

$ sudo make install
