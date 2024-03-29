# imu_visualization
IMU Sensor Visualization with ROS and Arduino Mega

This repository contains code to visualize IMU sensor data from an Arduino Mega connected to the BNO055 IMU sensor using ROS Noetic.

Prerequisites

    1.ROS Noetic installed (Installation Guide)
    2.Arduino Mega connected to the BNO055 IMU sensor
    3.rosserial_python package installed (Installation Guide)
    4.RViz installed (Installation Guide)

Setup

    1.Connect your Arduino Mega to the BNO055 IMU sensor.
    2.Clone this repository into your ROS workspace:

bash

    git clone https://github.com/Aakash872/imu_visualization.git

Open a terminal and run the rosserial serial node to establish communication between Arduino and ROS:

bash

rosrun rosserial_python serial_node.py /dev/ttyUSB0

Open another terminal and launch RViz with the pre-configured display for IMU visualization:

bash

    rviz -d imu_display.rviz

## Video Demonstration

Check out this video demonstrating the IMU sensor visualization:

[Direct link to video](https://drive.google.com/file/d/1jZdntY70H5puhPGzcmkoQJnDq_M82B4g/view?usp=sharing)


Notes

    1.Make sure your Arduino is properly configured to send IMU sensor data.
    2.The imu_display.rviz file contains the RViz configuration for visualizing the IMU sensor data. Adjust it according to your requirements.
    3.Modify the topic names in imu_display.rviz if your ROS topics differ from the defaults.

Contact

For any issues or suggestions, please contact:

    Aakash Tiwari - aakashtiwari07.12.2003@gmail.com
    Robotics Society, NIT Hamirpur - robonith@nith.ac.in