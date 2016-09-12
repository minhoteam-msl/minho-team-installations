#OpenCV Installation Guide

[Download online installer from http://opencv.org/]

[Open a terminal]

$ sudo apt-get -y remove ffmpeg x264 libx264-dev

$ sudo apt-get -y install libopencv-dev

$ sudo apt-get -y install build-essential checkinstall cmake pkg-config yasm

$ sudo apt-get -y install libjpeg-dev libjasper-dev

$ sudo apt-get -y install libavcodec-dev libavformat-dev libswscale-dev libdc1394-22-dev libgstreamer0.10-dev libgstreamer-plugins-base0.10-dev libv4l-dev

$ sudo apt-get -y install python-dev python-numpy

$ sudo apt-get -y install libtbb-dev

$ sudo apt-get -y install libqt4-dev libgtk2.0-dev

$ sudo apt-get -y install libfaac-dev libmp3lame-dev libopencore-amrnb-dev libopencore-amrwb-dev libtheora-dev libvorbis-dev libxvidcore-dev

$ sudo apt-get -y install x264 v4l-utils ffmpeg

####[Extract .zip file to ~ ]

$ cd opencv-[version]

$ mkdir build

$ cd build

$ cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local -D WITH_V4L=ON -D BUILD_EXAMPLES=ON -D WITH_OPENGL=ON ..

$ make -j$(nproc)

$ sudo make install

$ sudo sh -c 'echo "/usr/local/lib" > /etc/ld.so.conf.d/opencv.conf'

$ sudo ldconfig
