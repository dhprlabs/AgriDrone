# AgriDrone Project

## Overview

This project focuses on building a custom hexacopter drone with a thermal camera for monitoring tasks in agricultural fields. We started with an 
S550 hexacopter frame available online and assembled the drone myself to understand each subsystem and how all components work 
together in a real platform. The platform now includes an onboard NVIDIA Jetson Orin Nano for running ROS2 and integrating perception sensors 
like camera and LiDAR. The long-term goal is to build a complete autonomous ROS2-based drone stack that can be tested in simulation and then 
deployed on real hardware.

---

## Project Journey

1. Started from an S550 hexacopter frame.
2. Ordered individual drone parts and assembled everything manually.
3. Studied how propulsion, power, control, sensing, and communication interact.
4. Integrated a thermal camera for agriculture-focused monitoring use cases.
5. Began autonomous control development using ROS2.
6. Explored MAVROS and currently working on ROS2-based control of the drone.
7. Currently interfacing Intel RealSense D435i and LiDAR for field navigation.

---

## Hardware and Components

### Airframe and Propulsion

* Frame: S550 hexacopter frame
* Motors: Emax (935KV) Brushless DC motors (6x)
* ESCs: BLHeli LittleBee 30A ESC (6x)
* Propellers: Matched set for hexacopter configuration

### Power System

* Li-Po battery pack (GenX 4S 8000 mAh)
* Power distribution wiring/module

### Flight Control and Communication

* Flight Controller: Pixhawk 2.4.8
* Telemetry module
* Ground control station link

### Onboard Computing

* NVIDIA Jetson Orin Nano (onboard companion computer)
* Used for ROS2 runtime and sensor integration (camera, LiDAR, and processing pipeline)

### Sensors and Perception

* Thermal camera (agriculture monitoring)
* Intel RealSense D435i (in progress)
* LiDAR (in progress)
* IMU and (via flight controller stack)
* GPS (GOKU GM10 Pro V3)

---

## Software Stack

* ArduPilot flight stack for low-level flight control
* ROS2 for autonomy and higher-level control
* MAVROS for communication between ROS2 and autopilot
* Sensor integration pipeline for thermal, depth, and range data

---

## Current Status

* Hexacopter assembled and operational at hardware level
* Thermal camera integrated for monitoring tasks
* ROS2-based autonomous control development started
* MAVROS-based control pipeline under active development
* Jetson Orin Nano integrated as onboard compute for ROS2 and sensor stack
* RealSense D435i and LiDAR interfacing in progress

---

## Future Goals

### Near Term

* Complete stable ROS2 control through MAVROS
* Finalize RealSense D435i and LiDAR integration
* Build robust navigation capability for agricultural field scenarios

### Mid to Long Term

* Simulate the drone in a physics simulator to validate algorithms safely
* Test and benchmark autonomy modules in simulation before hardware deployment
* Port validated algorithms to the real drone platform
* Build a complete end-to-end ROS2 autonomy stack

---

## Media Placeholders

### Images

[Images folder link](https://drive.google.com/drive/folders/14M81Qpv3gCJgTJC6m3FQGDAzh3SMPkZq?usp=sharing)

### Videos

[Videos folder link](https://drive.google.com/drive/folders/19GkP9Q1G5dpIrfDLj3RhiwtsTNBPdRUC?usp=sharing)

---

## Author

- Dhairya Prajapati - [GitHub](https://github.com/dhprlabs)

- Devanshu Mangal - [GitHub](https://github.com/Mangal-Devanshu)
