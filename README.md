# Drowsy Eye Detection System 🚘😴

The **Drowsy Eye Detection System** is a real-time computer vision application designed to monitor the driver's eye movements through a camera. It helps prevent accidents caused by driver fatigue by detecting drowsiness and playing a buzzer sound to alert the driver.

---

## 🔍 How It Works

The system uses facial landmark detection to locate the eyes of the driver. It calculates the **Eye Aspect Ratio (EAR)** — a metric that decreases when eyes begin to close. If the EAR drops below a threshold for a number of consecutive frames, the system detects drowsiness and plays a warning beep using an audio file (`music.wav`).

---

## 🧠 Technologies Used

- **Python**
- **OpenCV** – for image processing and webcam feed
- **dlib** – for facial landmark prediction
- **imutils** – for easier frame handling
- **scipy** – to calculate distances between facial points
- **pygame** – to play alert sound

---

## 🛠️ Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/drowsy-eye-detection.git
   cd drowsy-eye-detection
   ```

2. **Install Dependencies**
   ```bash
   pip install opencv-python dlib imutils pygame scipy
   ```

3. **Download Required Model**
   - Download `shape_predictor_68_face_landmarks.dat` from the [official dlib model page](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2)
   - Extract the file and place it in the project directory

4. **Run the Program**
   ```bash
   python main.py
   ```

---

## 🚨 Features

- Real-time webcam monitoring of driver's eyes
- Calculates Eye Aspect Ratio (EAR)
- Alerts with buzzer when eyes are closed for too long
- Eye landmarks visualized on screen
- Easy-to-use and lightweight

---

## 📁 Project Structure

```
.
├── main.py
├── music.wav
├── shape_predictor_68_face_landmarks.dat
└── README.md
```

---

## 👤 Author

**Rupin Mallampalli**

---

## 📌 Future Enhancements

- Add GUI interface for better interaction
- Store session logs or driver behavior
- Integrate with car systems for automatic response

---

## ⚠️ Disclaimer

This project is intended as a **prototype** and should not be solely relied upon in critical driving environments. Always drive responsibly and stay alert.

---
