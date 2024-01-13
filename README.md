# Development-of-Autonomous-Mobile-Robot

We designed and implemented an autonomous mobile robot that can map and navigate outdoor environments. This was achieved through using multiple sensors including LIDAR, Stereo Camera, IMU and Wheel Encoders. All the readings and control actions were taken using packages in ROS-Noetic

## Sensors and Packages used
### LIDAR
We used the RPLIDAR-A3 from SLAMTEC. It has a relatively high sampling rate of 16kHz, and can work in both indoor and outdoor modes. We used the ROS-Notice Package from the SLAMTEC repository here: https://github.com/Slamtec/rplidar_ros/tree/master.
### Stereo Camera
We used the OAK-D Stereo Camera. It is well supported in the ROS community and has an on-board 9-axis IMU. We used the *depthai-ros* package from the luxonis repository here: https://github.com/luxonis/depthai-ros/tree/noetic
### IMU
We used the OAK-D on-board 9-axis IMU, which has embedded sensor fusion.
### Wheel Encoders
We used 360ppr Encoders which collected Odometry data. The odometry message was then fused with readings from the IMU, Visual-Odometry and ICP-odometry coming from the LIDAR.

## Flowchart

![image](https://github.com/mazenelgabalawy/Development-of-Autonomous-Mobile-Robot/assets/72276135/62c71a6a-cba6-4341-aaf7-1048d6c984c1)


## Results


https://github.com/mazenelgabalawy/Development-of-Autonomous-Mobile-Robot/assets/72276135/39a99236-3ba3-4207-9ca6-fda140f0fe0e

