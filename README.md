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

DroneAI is a portfolio-quality autonomous drone project built entirely in simulation using open-source technologies.

The project replicates the complete software stack of a modern autonomous drone—from flight control and telemetry to computer vision and AI decision-making—without requiring physical hardware.

The long-term goal is to migrate this software with minimal changes to real hardware such as a Raspberry Pi and Pixhawk/Cube Orange flight controller.

---

# 🎯 Project Objectives

- Build an autonomous drone completely in simulation
- Learn professional drone software architecture
- Integrate AI with autonomous flight
- Develop real-time computer vision capabilities
- Build an industry-ready robotics portfolio

---

# ✨ Features

## 🚁 Flight Control

- ✅ PX4 SITL Connection
- ✅ Drone Connection (MAVSDK)
- ✅ Arm
- ✅ Disarm
- ✅ Autonomous Takeoff
- ✅ Hover
- ✅ Autonomous Landing

---

## 📡 Telemetry

- ✅ Position
- ✅ Relative Altitude
- ✅ Velocity
- ✅ Flight Mode
- ✅ Battery Monitoring
- ✅ Real-Time Telemetry Logging

---

## 🛰 Autonomous Navigation

- ✅ Mission Framework
- ✅ GPS Navigation
- ✅ Waypoint Mission
- ✅ Return To Launch (RTL)
- ✅ Geofence Framework

---

## 👁 Computer Vision

- ✅ Gazebo Camera Integration
- ✅ OpenCV Live Streaming
- ✅ ArUco Marker Detection
- ✅ QR Code Detection
- ✅ YOLO Object Detection
- 🔄 Live YOLO Detection

---

## 🤖 AI (Upcoming)

- ⏳ AI Decision Engine
- ⏳ Object Tracking
- ⏳ Autonomous Following
- ⏳ Obstacle Avoidance
- ⏳ Autonomous Search Mission

---

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
DroneAI/
│
├── README.md
├── LICENSE
├── requirements.txt
├── .gitignore
│
├── docs/
│   ├── setup.md
│   ├── architecture.md
│   └── project_progress.md
│
├── scripts/
│   ├── arm.py
│   ├── disarm.py
│   ├── takeoff.py
│   ├── land.py
│   ├── telemetry.py
│   ├── mission.py
│   ├── camera_test.py
│   ├── aruco_test.py
│   ├── aruco_live.py
│   ├── qr_test.py
│   ├── generate_qr.py
│   ├── yolo_test.py
│   └── yolo_live.py
│
├── drone_control/
│   ├── connect.py
│   ├── action.py
│   └── telemetry.py
│
├── vision/
│   ├── camera_stream.py
│   ├── aruco_detection.py
│   ├── qr_detection.py
│   └── yolo_detection.py
│
├── config/
│   └── drone_config.py
│
├── tests/
│   └── test_connection.py
│
├── images/
│   ├── screenshots/
│   ├── vision/
│   └── yolo_results/
│
└── logs/
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/Fuad1103/DroneAI.git

cd DroneAI
```

Create virtual environment

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

# 📈 Project Roadmap

| Phase | Status |
|--------|--------|
| Environment Setup | ✅ Completed |
| PX4 + Gazebo | ✅ Completed |
| Flight Control | ✅ Completed |
| Advanced Telemetry | ✅ Completed |
| Autonomous Navigation | ✅ Completed |
| Computer Vision | 🟡 In Progress |
| AI Decision Engine | ⏳ Planned |
| LiDAR Navigation | ⏳ Planned |
| Autonomous Mission Planning | ⏳ Planned |
| Real Hardware Deployment | ⏳ Planned |

---

# 📊 Current Progress

## ✅ Completed

- PX4 SITL
- Gazebo Harmonic
- MAVSDK Integration
- Drone Connection
- Arm
- Disarm
- Takeoff
- Hover
- Landing
- Telemetry
- GPS
- Mission Framework
- Gazebo Camera
- OpenCV Streaming
- ArUco Detection
- QR Detection
- Static YOLO Detection

---

## 🔄 Currently Working On

- Live YOLO Detection from Gazebo Camera
- AI Decision Engine

---

## 🎯 Next Milestones

- Object Tracking
- Person Following
- Obstacle Avoidance
- Autonomous Navigation using AI
- Raspberry Pi Deployment
- Pixhawk Deployment

---

# 🧠 Skills Demonstrated

- Autonomous Drone Development
- PX4 SITL
- MAVSDK
- MAVLink
- Gazebo Simulation
- Python
- Computer Vision
- OpenCV
- YOLO
- ArUco Detection
- QR Code Detection
- Linux
- Git & GitHub
- Remote Development
- AI for Robotics

---

# 📷 Screenshots

Coming soon

- PX4 Simulation
- Gazebo World
- Takeoff
- Landing
- Camera Feed
- YOLO Detection

---

# 📹 Demo Video

Coming soon

---

# 👨‍💻 Author

**Fuad Bin Zafar**

M.Eng. Media Engineering with AI

Anhalt University of Applied Sciences

📧 Email: *(Add your email)*

🔗 LinkedIn: https://www.linkedin.com/in/fuad-bin-zafar/

💻 GitHub: https://github.com/Fuad1103

---

# 📄 License

This project is licensed under the MIT License.