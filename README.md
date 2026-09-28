# hand-gesture-robotic-arm
# Hand Gesture Controlled Robotic Arm 🤖🖐️

An interactive hardware-software project that controls a robotic arm using real-time human hand gestures captured via a webcam.

---

## 📌 Project Overview
This project maps hand keypoints detected by a camera into servo motor angles, allowing a robotic arm to mirror the user's hand movements in real time. It uses **MediaPipe** for hand tracking, **OpenCV** for image processing, and **Arduino** (or ESP32) for hardware execution.

---

## ✨ Features
- **Real-Time Hand Tracking:** Detects 21 hand landmarks using MediaPipe.
- **Gesture Control:**
  - Index finger movement controls joints (X/Y position).
  - Distance between Thumb and Index finger controls the **Gripper** (Open/Close).
  - Palm orientation controls wrist/base rotation.
- **Serial Communication:** Sends smooth angle data to Arduino via UART/Serial connection.
- **Smooth Servo Motion:** Includes angle smoothing logic to prevent sudden motor jerks.

---

## 🛠️ Hardware Requirements
- **Arduino Uno / ESP32**
- **4-DOF / 5-DOF Robotic Arm Kit**
- **Servo Motors** (e.g., SG90 or MG996R) x4–x6
- **External Power Supply** (5V / 3A-5A DC for servos)
- **Webcam** (Built-in or USB)
- **Breadboard & Jumper Wires**

---

## 💻 Software Requirements
- **Python 3.8+**
- **Arduino IDE**

### Required Python Packages
- `opencv-python`
- `mediapipe`
- `pyserial`
- `numpy`

---

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/hand-gesture-robotic-arm.git](https://github.com/your-username/hand-gesture-robotic-arm.git)
cd hand-gesture-robotic-arm
