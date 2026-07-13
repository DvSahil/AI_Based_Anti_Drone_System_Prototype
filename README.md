# 🛡️ AI-Powered Anti-Drone Detection & Tracking System

> **Real-Time Drone Detection • Intelligent Tracking • Computer Vision • Robotics • Automation**

<p align="center">

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-111827?style=for-the-badge)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-Uno-00979D?style=for-the-badge&logo=arduino&logoColor=white)

</p>

---

## 📖 Overview

This repository presents an **AI-driven anti-drone surveillance prototype** that combines **deep learning, computer vision, embedded systems, and automation**.

The system continuously monitors a live camera feed, detects drones using a **custom-trained YOLOv8 model**, estimates their position, and commands a pan-tilt mechanism through an Arduino-based controller to keep the target centered.

> **Note:** This repository focuses on **detection, tracking, and automation** for research and educational purposes.

## ✨ Features

- 🎯 Real-time drone detection
- 🤖 Automatic visual tracking
- 📷 Live webcam inference
- ⚡ Fast YOLOv8 inference
- 🔌 Arduino communication
- 🎥 Servo pan-tilt tracking
- 🧠 Modular AI pipeline

## 🏗️ Workflow

```text
Camera → YOLOv8 → Detection → Tracking → Arduino → Pan-Tilt Motion
```

## 📂 Repository Structure

```text
Anti-Drone-System/
├── assets/
├── src/
├── arduino/
├── dataset/
├── notebooks/
├── docs/
├── requirements.txt
└── README.md
```

## 🚀 Installation

```bash
git clone https://github.com/YOUR_USERNAME/Anti-Drone-System.git
cd Anti-Drone-System
pip install -r requirements.txt
python src/detect.py
```

## 🛠️ Tech Stack

| Area | Technology |
|------|------------|
| AI | YOLOv8 |
| Vision | OpenCV |
| DL | PyTorch |
| Hardware | Arduino Uno |
| Language | Python |

## 📈 Future Scope

- Multi-drone tracking
- ROS2 integration
- Edge AI deployment
- Thermal camera support

## 👨‍💻 Author

**Mohammad Sahil Khan**

B.Tech Mechanical Engineering, Jamia Millia Islamia

⭐ If you found this project useful, please give it a star.
