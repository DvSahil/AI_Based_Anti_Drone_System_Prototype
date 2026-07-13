# 🛰️ Autonomous Anti-Drone Detection & Tracking Platform

> **Vision-Based Drone Detection • Real-Time Object Tracking • Embedded Automation**

<p align="center">

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-111827?style=for-the-badge)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-Uno-00979D?style=for-the-badge&logo=arduino&logoColor=white)

</p>

---

## 📖 About the Project

This project is a prototype **counter-drone surveillance system** built around **computer vision, deep learning, and embedded hardware control**.

A live video feed is analyzed frame-by-frame using a **custom-trained YOLOv8 model** to detect aerial drones. Once a target is identified, the system calculates its relative position and drives a **pan-tilt servo mechanism** via an Arduino microcontroller to keep the drone centered in frame.

> **Disclaimer:** Built strictly for **research, learning, and prototyping** purposes — this is a detection & tracking demo, not a deployable defense system.

## ✨ Key Features

- 🎯 Real-time drone detection from live video
- 🤖 Closed-loop visual tracking
- 📷 Webcam-based inference pipeline
- ⚡ Lightweight, fast YOLOv8 inference
- 🔌 Serial communication with Arduino
- 🎥 Pan-tilt servo target following
- 🧠 Modular, extendable AI pipeline design

## 🏗️ System Workflow

```text
Camera Feed → YOLOv8 Inference → Target Localization → Tracking Logic → Arduino Serial Command → Pan-Tilt Servo Motion
```

## 📂 Project Structure

```text
Anti-Drone-System/
├── assets/          # Images, sample outputs, demo media
├── src/             # Core detection & tracking scripts
├── arduino/         # Arduino sketches for servo control
├── dataset/         # Training/validation data
├── notebooks/       # Experiment & training notebooks
├── docs/            # Documentation
├── requirements.txt
└── README.md
```

## 🚀 Getting Started

```bash
git clone https://github.com/YOUR_USERNAME/Anti-Drone-System.git
cd Anti-Drone-System
pip install -r requirements.txt
python src/detect.py
```

## 🛠️ Tech Stack

| Component | Tool/Framework |
|-----------|----------------|
| Object Detection | YOLOv8 |
| Computer Vision | OpenCV |
| Deep Learning Backend | PyTorch |
| Microcontroller | Arduino Uno |
| Core Language | Python |

## 📈 Roadmap

- [ ] Multi-drone simultaneous tracking
- [ ] ROS2 integration for robotic platforms
- [ ] Edge AI deployment (Jetson/Coral)
- [ ] Thermal camera support for low-visibility detection

## 👨‍💻 Author

**Mohammad Sahil Khan**
B.Tech Mechanical Engineering, Jamia Millia Islamia

If this project helped you, consider giving it a ⭐!
