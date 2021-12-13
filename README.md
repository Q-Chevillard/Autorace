# Autorace
![image](https://user-images.githubusercontent.com/62595618/145738760-61a1fe0c-c297-4c03-8b36-6aabd3469caa.png)

## Technical documentation
[Technical documentation](https://github.com/Q-Chevillard/Autorace/blob/511b83aabb3bfb0c0444316ae1cb6c88e4e65f3f/Technical%20Documentation.pdf)

## Related medias
[google drive](https://drive.google.com/drive/folders/1oEMVAOJoUQk3slDalRYiPA_bhgDXfmDj?usp=sharing)

## User manual
### Installation
The following instructions describes how to install packages and to calibrate camera.

1. Install Autorace package on both Remote PC and SBC.
   ```cd ~/catkin_ws/src/
   git clone -b kinetic-devel https://github.com/Q-Chevillard/Autorace.git
   cd ~/catkin_ws && catkin_make```


2. Install additional dependent packages on Remote PC.

```sudo apt-get install ros-kinetic-image-transport ros-kinetic-cv-bridge ros-kinetic-vision-opencv python-opencv libopencv-dev ros-kinetic-image-proc```

### Launch autorace
1. Launch roscore in **remote PC**
   ```roscore```

2. Bringup the robot in **ssh**
   ```roslaunch turtlebot3_bringup turtlebot3_robot.launch```
   
3. Start the camera in **ssh**
   ```roslaunch turtlebot3_autorace_traffic_light_camera turtlebot3_autorace_camera_pi.launch```
   
if you want just launch the lane following do the 4.1 step, else if you want to launch the traffic light mission and the following lane do the step 4.2.

4.1 launch the lane follower launcher script in **remote PC**
   ```./<directory>/lane_follower_launcher.sh```

4.2 launch the traffic light launcher script in **remote PC**
   ```./<directory>/traffic_light_launcher.sh```
