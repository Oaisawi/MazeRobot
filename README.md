# Autonomous Maze Solving Robot with ROS 2, LIDAR, and Gazebo

This project simulates an autonomous robot that navigates through a maze using real-time LIDAR sensor data and a simple wall-following algorithm. The robot is deployed in a Gazebo simulation environment and is controlled using ROS 2. It operates without any preloaded map, relying entirely on reactive decision-making through sensor input.

## Features

- Simulated robot in a custom maze environment using Gazebo
- 2D LIDAR-based obstacle detection
- Wall-following maze solving algorithm (left-hand rule)
- Modular architecture with ROS 2 nodes
- RViz visualization for LIDAR data and robot movement
- Lightweight and educationally focused codebase

## Prerequisites

- Ubuntu 22.04
- ROS 2 Humble Hawksbill
- Gazebo (comes with ros-humble-desktop)
- Python 3.10+
- colcon, rosdep, git

### Install Dependencies

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install -y ros-humble-desktop \
  python3-colcon-common-extensions \
  python3-rosdep \
  python3-pip \
  python3-vcstool \
  build-essential \
  ros-humble-gazebo-ros-pkgs \
  ros-humble-gazebo-ros2-control

sudo rosdep init 2>/dev/null || true
rosdep update
