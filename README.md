# Intelligent-Ground-Vehicle
Intelligent Ground Vehicle (IGV) is an autonomous rover developed for ROBOFEST Gujarat, designed to navigate complex terrains using a modified rocker suspension and ROS2-based autonomy. It integrates LiDAR, RGB-D vision, GNSS, and SLAM for reliable, collision-free navigation

📌 Overview

The Intelligent Ground Vehicle (IGV) project focuses on the design and development of an autonomous rover capable of navigating complex, unstructured terrains with minimal human intervention. Developed for the ROBOFEST Gujarat – Ground Vehicle Category, the rover demonstrates robust mechanical design, advanced perception, and autonomous navigation using ROS2-based software architecture.
This project addresses real-world challenges in autonomous navigation, where robots must operate reliably in cluttered, constrained, and dynamic environments, such as disaster zones, agricultural fields, and outdoor terrains.

🎯 Objectives
- Design a stable and lightweight rover platform for rough terrain traversal
- Achieve collision-free autonomous navigation across multi-stage obstacle courses
- Integrate sensor fusion, SLAM, and path planning using ROS2
- Validate performance through simulation (Gazebo + RViz) and real-world testing

  🏁 Competition Context

The Ground Vehicle Category consists of four progressive stages, each increasing in obstacle density and terrain complexity. Performance is evaluated based on:
- Collision-free navigation success rate
- Shortest traversal time
- Autonomy, robustness, and reliability
  
🛠️ Mechanical Design

- Suspension System: Modified Double Rocker Mechanism
- Chassis Material: Aluminum Alloy 6063-T6 (extrusion grade)

- Dimensions:

  - Length: 83.8 cm

  - Width: 69 cm

  - Height: 60 cm

- Terrain Capability:

  - Climbs slopes up to 45°
  - Maintains continuous wheel–ground contact
- Validation:
  - FEA confirms max deformation ≈ 0.0012 mm
  - Factor of Safety: 2.0 – 2.5
    
⚙️ Electronics & Sensors

- Low-Level Controller: Custom ESP32-S3 PCB

- High-Level Computer: NVIDIA Jetson Orin Nano

- Sensors:

  - YDLIDAR G2 (360° LiDAR)

  - Intel RealSense D435i (RGB-D + IMU)

  - MPU-9250 (9-axis IMU)

  - GNSS (u-blox M10)

  - Wheel Encoders (600 PPR)

🤖 Software Architecture

- Framework: ROS2

- Core Modules:

  - Sensor fusion (EKF)

  - 2D/3D SLAM (Cartographer, RTAB-Map)

  - Navigation stack (Nav2)

- Operating Modes:

  - Manual (PS5 controller)

  - Semi-autonomous

  - Fully autonomous

🧪 Simulation & Digital Twin

A Gazebo-based digital twin was developed to validate:

- Line following (Stage 1)

- Obstacle avoidance

- Ramp climbing

- Dynamic obstacle handling

Visualization and debugging were performed using RViz2 and RQT.
  
