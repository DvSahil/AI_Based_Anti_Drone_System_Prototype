# 🛡️ AI-Powered Anti-Drone Detection & Tracking System

> Real-time drone detection and automated tracking using **YOLOv8**, **OpenCV**, **Python**, and **Arduino**.

![Python](https://img.shields.io/badge/Python-3.8+-blue)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Ultralytics-red)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green)
![Arduino](https://img.shields.io/badge/Arduino-Uno-teal)
![License](https://img.shields.io/badge/License-MIT-orange)

---

# 📖 Overview

This project presents an intelligent anti-drone surveillance system capable of detecting, tracking, and responding to unauthorized drones in real time.

A custom-trained **YOLOv8** object detection model identifies drones from a live camera feed. Once detected, the target's position is continuously monitored, allowing an Arduino-controlled pan-tilt platform to automatically align with the drone. The system is designed as a research prototype demonstrating the integration of computer vision, embedded systems, and automation.

---

# ✨ Features

- Real-time drone detection using YOLOv8
- Live object tracking with OpenCV
- Automatic pan-tilt tracking using servo motors
- Serial communication between Python and Arduino
- Target lock detection based on object position
- Modular architecture for future AI upgrades
- Custom dataset trained specifically for drone detection

---

# 🏗️ System Architecture

```
Camera
   │
   ▼
YOLOv8 Detection
   │
Bounding Box
   │
Object Center Calculation
   │
Tracking Algorithm
   │
Serial Communication
   │
Arduino UNO
   │
Pan-Tilt Servo System
```

---

# 🧠 AI Pipeline

The complete workflow consists of:

### 1. Image Acquisition
A USB camera continuously captures live video frames.

### 2. Drone Detection
Each frame is processed using a custom-trained YOLOv8 model that detects drones and generates bounding boxes with confidence scores.

### 3. Position Estimation
The center coordinates of the detected drone are calculated and compared with the center of the camera frame.

### 4. Tracking
Horizontal and vertical errors are computed to determine the movement required by the servos.

### 5. Hardware Control
Movement commands are transmitted to the Arduino through serial communication, enabling smooth pan and tilt tracking.

---

# 📂 Project Structure

```
Anti-Drone-System/

│── assets/
│── arduino/
│── configs/
│── dataset/
│── docs/
│── notebooks/
│── scripts/
│── src/
│── requirements.txt
│── README.md
│── LICENSE
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Anti-Drone-System.git
```

Move into the project folder

```bash
cd Anti-Drone-System
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Running the Project

### Train the Model

```bash
python src/train.py
```

### Run Real-Time Detection

```bash
python src/detect.py
```

### Upload Arduino Code

Open the Arduino sketch inside the **arduino/** folder and upload it to your Arduino Uno.

---

# 🧩 Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Main programming language |
| YOLOv8 | Drone detection |
| OpenCV | Image processing |
| PyTorch | Deep learning framework |
| Arduino UNO | Hardware controller |
| Serial Communication | PC-Arduino interface |
| Roboflow | Dataset management |

---

# 📊 Model Performance

| Metric | Result |
|---------|--------|
| Detection Accuracy | High |
| Real-Time Speed | 18–25 FPS |
| Response Time | Less than 1 second |
| Confidence Score | Typically above 0.80 |

---

# 🔧 Hardware Components

- Arduino Uno
- HD USB Camera
- 2 × MG996R Servo Motors
- Pan-Tilt Mount
- USB Cable
- External Power Supply
- Relay Module (Optional)
- Spark Module (Prototype Demonstration)

---

# 📈 Workflow

```
Live Camera Feed
        │
        ▼
YOLOv8 Detects Drone
        │
        ▼
Calculate Drone Position
        │
        ▼
Generate Tracking Commands
        │
        ▼
Send Commands to Arduino
        │
        ▼
Servo Motors Follow Target
```

---

# 📸 Sample Output

The system displays:

- Drone bounding box
- Confidence score
- Target center
- Tracking status
- Real-time FPS

---

# 🎯 Applications

- Border surveillance
- Restricted area monitoring
- Research and education
- Industrial security
- Smart surveillance systems
- Autonomous defense research

---

# 🔮 Future Improvements

- Multi-drone detection
- Thermal camera support
- Kalman Filter based prediction
- Edge AI deployment using Jetson Nano
- Radar and vision sensor fusion
- GPS-based tracking
- Automatic alert system
- Cloud monitoring dashboard

---

# 📚 Learning Outcomes

This project demonstrates practical implementation of:

- Deep Learning
- Computer Vision
- Embedded Systems
- Robotics
- Automation
- Object Detection
- Serial Communication
- Real-Time Control Systems

---

# 🤝 Contributing

Contributions are welcome.

You can contribute by:

- Improving detection accuracy
- Optimizing tracking algorithms
- Adding new datasets
- Enhancing documentation
- Reporting bugs
- Suggesting new features

---

# 📄 License

This project is released under the MIT License.

---

# 👨‍💻 Author

**Mohammad Sahil Khan**

B.Tech Mechanical Engineering  
Jamia Millia Islamia, New Delhi

**Areas of Interest**

- Robotics
- Artificial Intelligence
- Computer Vision
- Automation
- UAV Systems
- Autonomous Robotics

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
