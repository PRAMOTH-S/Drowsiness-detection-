# 😴 Driver Drowsiness Detection System

A real-time **Driver Drowsiness Detection System** built using **Python, OpenCV, and dlib**.  
This system monitors eye activity using facial landmarks and detects drowsiness based on the **Eye Aspect Ratio (EAR)**. When prolonged eye closure is detected, an alert is triggered.

---

## 📌 Overview

Driver fatigue is a major cause of road accidents. This project provides a **computer vision-based solution** that detects drowsiness in real time using a webcam and alerts the user.

---

## 🔗 Repository Link

👉 **[View Project on GitHub](https://github.com/PRAMOTH-S/drowsiness-detection)**

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

1. Capture video from webcam  
2. Convert frame to grayscale  
3. Detect face using dlib  
4. Extract facial landmarks  
5. Track eye regions  
6. Calculate EAR  
7. Trigger alert if EAR stays below threshold  

---

## 📊 Eye Aspect Ratio (EAR)

```
EAR = (||p2 - p6|| + ||p3 - p5||) / (2 × ||p1 - p4||)
```

---

## 🛠️ Tech Stack

- **Python**
- **OpenCV**
- **dlib**
- **imutils**
- **scipy**

---

## 📦 Installation

```bash
git clone https://github.com/PRAMOTH-S/drowsiness-detection.git
cd drowsiness-detection
pip install opencv-python dlib imutils scipy
```

---

## ⚠️ Setup Notes

- Install **Visual C++ Build Tools** before installing `dlib`
- `winsound` is built-in (Windows only)
- No need for `sklearn`

---

## 📁 Required File

```
shape_predictor_68_face_landmarks.dat
```

📌 Place this file in the same directory as `main.py`

---

## ▶️ Run

```bash
python main.py
```

Press **Q** to exit.

---

## ⚙️ Configuration

```python
earThresh = 0.3
earFrames = 48
```

---

## 🔔 Alert

- On-screen warning: **DROWSINESS DETECTED**
- Beep sound using system audio

---

## ⚠️ Limitations

- Needs proper lighting  
- Requires frontal face  
- Windows-only sound  

---

## 🔮 Future Scope

- Deep learning enhancement  
- Mobile integration  
- Night-time detection  

---

## 👨‍💻 Author

**Pramoth S**  
🔗 https://github.com/PRAMOTH-S  

---

## ⭐ Support

If you found this useful, please give it a ⭐ on GitHub!
