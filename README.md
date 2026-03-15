# 😴 Driver Drowsiness Detection Syste

A real-time **Driver Drowsiness Detection System** built using **Python, OpenCV, and dlib**.  
This system monitors eye activity using facial landmarks and detects drowsiness based on the **Eye Aspect Ratio (EAR)**. When prolonged eye closure is detected, an alert is triggered.

---

## 📌 Overview

Driver fatigue is a significant cause of road accidents. This project provides a **computer vision-based solution** that detects drowsiness in real time using a webcam and alerts the user.

---

## 🚀 Features

- Real-time face detection using webcam  
- Facial landmark detection (68-point model)  
- Eye tracking using Eye Aspect Ratio (EAR)  
- Drowsiness detection using frame threshold logic  
- Visual alert + sound notification  
- Lightweight and efficient  

---

## 🧠 Methodology

1. Capture live video from webcam  
2. Convert frame to grayscale  
3. Detect face using dlib  
4. Extract 68 facial landmarks  
5. Identify left and right eye regions  
6. Compute Eye Aspect Ratio (EAR)  
7. Trigger alert if EAR remains below threshold for consecutive frames  

---

## 📊 Eye Aspect Ratio (EAR)

```
EAR = (||p2 - p6|| + ||p3 - p5||) / (2 × ||p1 - p4||)
```

- EAR decreases when eyes close  
- Continuous low EAR indicates drowsiness  

---

## 🛠️ Tech Stack

- **Language:** Python  
- **Libraries:** OpenCV, dlib, imutils, scipy  
- **Hardware:** Webcam  

---

## 📦 Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/PRAMOTH-S/drowsiness-detection.git
cd drowsiness-detection
```

### 2️⃣ Install Required Libraries

```bash
pip install opencv-python dlib imutils scipy
```

---

## ⚠️ Important Setup Notes

- Install **Visual C++ Build Tools** before installing `dlib` (Windows)
- `winsound` is built-in (no installation required)
- Do NOT install `sklearn` (not used)

---

## 📁 Required Model File

```
shape_predictor_68_face_landmarks.dat
```

### 🔽 Instructions

- Place this file in the **same folder as `main.py`**
- File name must match exactly

---

## 📂 Project Structure

```
drowsiness-detection/
│── main.py
│── shape_predictor_68_face_landmarks.dat
│── README.md
```

---

## ▶️ Run the Project

```bash
python main.py
```

- Press **Q** to exit  

---

## ⚙️ Configuration

```python
earThresh = 0.3
earFrames = 48
```

---

## 🔔 Alert Mechanism

- Displays: **DROWSINESS DETECTED**  
- Plays alert sound using `winsound`  

---

## ⚠️ Limitations

- Requires good lighting  
- Needs frontal face  
- Not for multiple faces  
- Sound works only on Windows  

---

## 🔮 Future Improvements

- Deep learning-based detection  
- Mobile integration  
- Night vision support  

---

## 👨‍💻 Author

**Pramoth S**  
https://github.com/PRAMOTH-S  

---

## ⭐ Support

If you found this useful, give it a ⭐ on GitHub!
