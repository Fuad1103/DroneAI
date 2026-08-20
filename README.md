# 🚁 DroneAI
## Autonomous Edge-AI Drone Platform using PX4, Gazebo, MAVSDK, OpenCV & YOLO

![Python](https://img.shields.io/badge/Python-3.12-blue)
![PX4](https://img.shields.io/badge/PX4-SITL-green)
![Gazebo](https://img.shields.io/badge/Gazebo-Harmonic-orange)
![MAVSDK](https://img.shields.io/badge/MAVSDK-Python-blueviolet)
![YOLO](https://img.shields.io/badge/YOLO-v11-red)
![OpenCV](https://img.shields.io/badge/OpenCV-5.x-success)
![Status](https://img.shields.io/badge/Status-Active-success)

---

# 📖 Overview

DroneAI is a portfolio-grade autonomous drone platform developed entirely in simulation using open-source technologies.

The project combines PX4 Autopilot, Gazebo Harmonic, MAVSDK-Python, OpenCV, YOLO11, and AI-based decision-making to simulate the software stack of a modern autonomous drone.

The system performs autonomous flight, waypoint navigation, obstacle detection, AI perception, sensor fusion, target tracking, and complete autonomous missions without requiring physical hardware.

The architecture is designed so the software can later be deployed with minimal modifications to real hardware such as Raspberry Pi, Pixhawk/Cube Orange+, cameras, and LiDAR sensors.

# 🎯 Project Objectives

- Build an autonomous drone completely in simulation
- Learn professional drone software architecture
- Integrate AI with autonomous flight
- Develop real-time computer vision capabilities
- Build an industry-ready robotics portfolio

---

# ✨ Features

## 🚁 Flight Control

- ✅ PX4 SITL
- ✅ MAVSDK Connection
- ✅ Arm / Disarm
- ✅ Automatic Takeoff
- ✅ Hover
- ✅ Automatic Landing
- ✅ Return To Launch (RTL)

---

## 📡 Telemetry

- ✅ GPS Position
- ✅ Relative Altitude
- ✅ Velocity
- ✅ Flight Mode
- ✅ Battery Monitoring
- ✅ Live Telemetry
- ✅ CSV Logging

---

## 🛰 Autonomous Navigation

- ✅ Waypoint Missions
- ✅ Mission Framework
- ✅ Mission State Machine
- ✅ GPS Navigation
- ✅ Offboard Navigation
- ✅ Return To Launch
- ✅ Intelligent Navigation Controller

---

## 👁 Computer Vision

- ✅ Gazebo Camera
- ✅ OpenCV Streaming
- ✅ YOLO11 Object Detection
- ✅ ArUco Detection
- ✅ QR Code Detection
- ✅ Live Vision Pipeline

---

## 📡 LiDAR

- ✅ Gazebo 2D LiDAR
- ✅ LaserScan Processing
- ✅ Directional Distance Detection
- ✅ Obstacle Detection
- ✅ Collision Warning
- ✅ Autonomous Avoidance

---

## 🤖 Artificial Intelligence

- ✅ Sensor Fusion
- ✅ AI Decision Engine
- ✅ Target Tracking
- ✅ Intelligent Navigation
- ✅ Live AI Brain
- ✅ Autonomous Mission Logic

---

## 🚀 Autonomous Mission

- ✅ Automatic Takeoff
- ✅ Waypoint Navigation
- ✅ AI Search Mode
- ✅ Mission State Machine
- ✅ RTL
- ✅ Automatic Landing

# 🏗 System Architecture

```
                DroneAI

         +--------------------+
         |   Python AI Layer  |
         | MAVSDK + OpenCV    |
         | YOLO + AI Logic    |
         +---------+----------+
                   |
             MAVLink / MAVSDK
                   |
         +---------+----------+
         |        PX4         |
         | Flight Controller  |
         +---------+----------+
                   |
              Gazebo Harmonic
                   |
      +------------+------------+
      |                         |
   RGB Camera               Sensors
   (OpenCV)                 GPS / IMU
```

---

# 🛠 Tech Stack

### Flight Control

- PX4 Autopilot
- MAVSDK-Python
- MAVLink

### Simulation

- Gazebo Harmonic
- PX4 SITL

### AI & Computer Vision

- Python
- OpenCV
- YOLO11
- NumPy
### AI

- YOLO11
- OpenCV
- NumPy
- Sensor Fusion
- AI Decision Engine

### Robotics

- PX4
- MAVSDK
- MAVLink
- Gazebo Harmonic

### Development

- Ubuntu 24.04 (UTM)
- VS Code Remote SSH
- Git
- GitHub

---

# 💻 Development Environment

### Hardware

- Apple MacBook Pro (Apple Silicon)

### Host OS

- macOS

### Virtual Machine

- Ubuntu 24.04 LTS (UTM)

### IDE

- VS Code (Remote SSH)

---

# 📂 Project Structure

```
ai/
├── decision_engine.py
├── intelligent_navigation.py
├── mission_state.py
├── navigation_controller.py
├── perception.py
├── sensor_fusion.py
├── target_follower.py
└── target_tracker.py

lidar/
├── lidar_reader.py
├── obstacle_detection.py
├── avoidance.py
└── lidar_utils.py

drone_control/
├── connect.py
├── action.py
├── mission.py
└── telemetry.py

simulation/
└── models/
    └── lidar_obstacle.sdf

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/Fuad1103/DroneAI.git

cd DroneAI
```

Create a virtual environment

```bash
python3 -m venv venv

source venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶ Running the Project

### Start PX4

```bash
cd ~/PX4-Autopilot

make px4_sitl gz_x500_mono_cam
```

---

### Test Connection

```bash
python3 -m tests.test_connection
```

---

### Arm Drone

```bash
python3 -m scripts.arm
```

---

### Takeoff

```bash
python3 -m scripts.takeoff
```

---

### Land

```bash
python3 -m scripts.land
```

---

### Camera Test

```bash
python3 -m scripts.camera_test
```

---

### ArUco Detection

```bash
python3 -m scripts.aruco_live
```

---

### QR Detection

```bash
python3 -m scripts.qr_test
```

---

### YOLO Detection

```bash
python3 -m scripts.yolo_test
```

---

### Live YOLO

```bash
python3 -m scripts.yolo_live
```

---
### Autonomous Mission

```bash
python3 -m scripts.autonomous_mission

###Live AI Brain
python3 -m scripts.live_ai_brain

###LiDAR Test
python3 -m scripts.lidar_test

###Obstacle Detection
python3 -m scripts.obstacle_test

###AI Decision Test
python3 -m scripts.decision_test


---

# Roadmap

Replace with:

| Phase | Status |
|--------|--------|
| Phase 1 – Development Environment | ✅ |
| Phase 2 – PX4 Flight Control | ✅ |
| Phase 3 – Telemetry System | ✅ |
| Phase 4 – Autonomous Navigation | ✅ |
| Phase 5 – Computer Vision | ✅ |
| Phase 6 – LiDAR & Obstacle Avoidance | ✅ |
| Phase 7 – AI Decision Engine | ✅ |
| Phase 8 – Complete Autonomous Mission | ✅ |
| Phase 9 – Mission Logging & Analytics | 🔄 |
| Phase 10 – Real Hardware Deployment | ⏳ |

---

# Current Progress

Replace with:

```markdown
# 📊 Current Progress

## ✅ Completed

- PX4 SITL
- Gazebo Harmonic
- MAVSDK Integration
- Flight Control
- Autonomous Takeoff
- Hover
- Landing
- GPS Navigation
- Waypoint Missions
- Return-To-Launch
- Camera Streaming
- OpenCV
- YOLO11 Detection
- ArUco Detection
- QR Detection
- LiDAR Processing
- Obstacle Detection
- Collision Warning
- AI Decision Engine
- Sensor Fusion
- Intelligent Navigation
- Target Tracking
- Complete Autonomous Mission

---

## 🔄 Currently Working On

- Mission Logging
- Performance Analytics
- Mission Replay
- Portfolio Demo Videos

---

## 🎯 Next Milestones

- Mission Analytics Dashboard
- ROS2 Integration
- SLAM
- Multi-Drone Coordination
- Raspberry Pi Deployment
- Pixhawk Deployment
---

###Skills Demonstrated
- Sensor Fusion
- AI Decision Making
- Autonomous Navigation
- LiDAR Processing
- Mission Planning
- Offboard Control
- Autonomous Robotics


# 📹 Demo Video

Coming soon

---

# 👨‍💻 Author

# 👨‍💻 Author

**Fuad Bin Zafar**

M.Eng. Media Engineering with AI  
Anhalt University of Applied Sciences

📧 Email: fuad110398@gmail.com

💻 GitHub: https://github.com/Fuad1103

🌐 Portfolio: https://fuadbinzafar.vercel.app

🔗 LinkedIn: https://www.linkedin.com/in/fuad1103/
---

# 📄 License
