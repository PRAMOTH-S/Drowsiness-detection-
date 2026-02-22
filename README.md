# 😴 Driver Drowsiness Detection System

A real-time **Driver Drowsiness Detection System** built using **Python, OpenCV, and dlib**.  
The system monitors eye movements using facial landmarks and detects drowsiness based on the **Eye Aspect Ratio (EAR)**. When prolonged eye closure is detected, an alert is triggered.

---

## 📌 Overview

Driver fatigue is a major cause of road accidents. This project implements a lightweight computer vision solution that continuously tracks eye activity and detects drowsiness in real time using a webcam.

---

## 🚀 Key Features

- Real-time face detection
- Facial landmark detection (68-point model)
- Eye tracking using EAR (Eye Aspect Ratio)
- Drowsiness detection based on frame threshold
- Visual alert + sound notification
- Lightweight and efficient

---

## 🧠 Methodology

The system follows this pipeline:

1. Capture video stream from webcam  
2. Convert frames to grayscale  
3. Detect face using dlib  
4. Extract facial landmarks  
5. Isolate left and right eye regions  
6. Compute Eye Aspect Ratio (EAR)  
7. Trigger alert if EAR remains below threshold  

---

## 📊 Eye Aspect Ratio (EAR)

\[
EAR = \frac{||p2 - p6|| + ||p3 - p5||}{2 \times ||p1 - p4||}
\]

- EAR decreases when eyes close  
- Continuous low EAR indicates drowsiness  

---

## 🛠️ Tech Stack

- **Language:** Python  
- **Libraries:**  
  - OpenCV  
  - dlib  
  - imutils  
  - scipy  
- **System Requirement:** Webcam  

---

## 📦 Installation

### 1. Clone Repository
```bash
git clone https://github.com/PramothS/drowsiness-detection.git
cd drowsiness-detection
