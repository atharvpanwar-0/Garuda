# Garuda
Autonomous Drone-Based Infrastructure Inspection System "An autonomous drone solution using Raspberry Pi 5 and YOLOv11-Nano for real-time, automated defect detection in industrial infrastructure. Built for BGI Hackathon 2026."
Project Title: Autonomous Drone-Based Infrastructure Inspection System
Overview
An intelligent, end-to-end automated solution designed for the safe and efficient inspection of critical infrastructure (power lines, bridges, and industrial pipelines).

Utilizes a combination of computer vision and autonomous flight planning to identify structural defects without human intervention.

Developed as a core entry for the BGI Hackathon 2026, focusing on reducing manual risk and increasing inspection frequency.

Key Features
Autonomous Navigation: Utilizes Pixhawk-based flight controllers integrated with custom waypoint algorithms to ensure precise coverage of target zones.

Real-time Defect Detection: Employs YOLOv11-Nano for high-speed, onboard inference to detect cracks, rust, and structural degradation in real-time.

Companion Computing: Powered by Raspberry Pi 5, enabling edge processing to minimize latency between capture and analysis.

Data Logging & Reporting: Automatically tags identified defects with precise GPS coordinates, generating an inspection report for maintenance crews.

Technical Architecture
Hardware Stack: * Flight Controller: Pixhawk (ArduPilot/PX4 firmware).

Processing Unit: Raspberry Pi 5.

Vision System: High-definition camera module optimized for low-latency streaming.

Software Stack:

Computer Vision: YOLOv11-Nano (optimized via OpenVINO or TensorRT).

Communication: MAVLink protocol for telemetry and drone control.

Language: Python (for integration logic and inference orchestration).

OS: Ubuntu 24.04 (Robot Operating System - ROS 2).

System Workflow
Mission Setup: Define mission parameters and waypoints via GCS (Ground Control Station).

Autonomous Flight: The drone navigates the path; data is captured via the onboard camera.

Edge Inference: The Raspberry Pi processes frames locally; detected anomalies are flagged immediately.

Data Transmission: Relevant clips and metadata are stored and synced for post-mission review.
