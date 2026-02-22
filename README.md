# 😴 Driver Drowsiness Detection System

A real-time **Driver Drowsiness Detection System** built using **Python, OpenCV, and dlib**.  
This project detects eye closure using facial landmarks and alerts the driver when drowsiness is detected.

---

## 🚀 Features

- Real-time face detection using webcam
- Eye tracking using facial landmarks (dlib)
- Eye Aspect Ratio (EAR) calculation
- Detects prolonged eye closure (drowsiness)
- Alert system using sound (beep)

---

## 🧠 How It Works

1. Capture live video from webcam  
2. Convert frame to grayscale  
3. Detect face using dlib  
4. Extract facial landmarks (68 points)  
5. Identify eye coordinates  
6. Compute **Eye Aspect Ratio (EAR)**  
7. If EAR < threshold for consecutive frames → trigger alert  

---

## 📦 Required Libraries

Install the following libraries before running the project:

```bash id="libs01"
pip install opencv-python
pip install dlib
pip install imutils
pip install scipy
