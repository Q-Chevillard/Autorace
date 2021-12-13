# Autorace
![image](https://user-images.githubusercontent.com/62595618/145738760-61a1fe0c-c297-4c03-8b36-6aabd3469caa.png)

## Technical documentation

## Related medias
https://drive.google.com/drive/folders/1oEMVAOJoUQk3slDalRYiPA_bhgDXfmDj?usp=sharing

## User manual
### Installation
The following instructions describes how to install packages and to calibrate camera.

1. Install AutoRace package on both Remote PC and SBC.
   cd ~/catkin_ws/src/
   git clone -b kinetic-devel https://github.com/Q-Chevillard/Autorace.git
   cd ~/catkin_ws && catkin_make


2. Install additional dependent packages on Remote PC.
sudo apt-get install ros-kinetic-image-transport ros-kinetic-cv-bridge ros-kinetic-vision-opencv python-opencv libopencv-dev ros-kinetic-image-proc
