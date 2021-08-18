# Calibration
In this repository, I'll show the Calibration Tools used.
Including single-camera calibration and camera-radar joint calibration in Autoware.

# Use steps 
## 1.Create a workspace 
```
mkdir -p catkin_ws/src
cd catkin_ws
catkin_make
```
## 2.Clone Calibration package 
```
cd ~/catkin_ws/src
git clone 
cd ..
catkin_make
```
## 3.Use calibration tools 
```
cd ~/catkin_ws
source devel/setup.bash
rosrun autoware_camera_lidar_calibrator cameracalibrator.py --square 0.1 --size 9x8 image:=/pylon_image/image_raw  //Single camera calibration tool 
rosrun calibration_camera_lidar calibrationtoolkit  //Camera lidar joint calibration 

```
