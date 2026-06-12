# Heart Rate & Eye Blink Detection Using Computer Vision

## 📌 Project Overview

This project is a real-time **Heart Rate Monitoring and Eye Blink Detection System** using a webcam. The system captures a user's face, detects facial landmarks, estimates heart rate using facial skin color variations (Remote Photoplethysmography - rPPG), and counts eye blinks using eye aspect ratio (EAR).

The project is developed using **Python, OpenCV, MediaPipe, NumPy, and SciPy**.

---

## 🚀 Features

* Real-time face detection
* Facial landmark detection using MediaPipe Face Mesh
* Eye blink detection and blink counting
* Heart rate estimation from facial region
* Live webcam feed
* Real-time visualization
* Forehead-based pulse signal extraction
* BPM (Beats Per Minute) calculation
* Lightweight and easy to run

---

## 🛠️ Technologies Used

* Python 3.10
* OpenCV
* MediaPipe
* NumPy
* SciPy
* Matplotlib
* Flask (optional web interface)

---

## 📂 Project Structure

```text
HeartRate_Blink_Project/
│
├── app.py
├── requirements.txt
│
├── modules/
│   ├── face_detector.py
│   ├── blink_detector.py
│   └── heart_rate.py
│
├── static/
│   └── style.css
│
├── templates/
│   └── index.html
│
└── README.md
```

## ⚙️ Installation

### 1. Clone Repository

```bash
git clone https://github.com/your-username/HeartRate_Blink_Project.git
cd HeartRate_Blink_Project
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

### 3. Activate Virtual Environment

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

```bash
python app.py
```

If using Flask:

```bash
python app.py
```

Open browser:

```text
http://127.0.0.1:5000
```

---

## 💡 Working Principle

### Face Detection

The webcam captures video frames and detects the user's face using OpenCV and MediaPipe.

### Eye Blink Detection

Eye landmarks are extracted from the face mesh.

Eye Aspect Ratio (EAR) is calculated to determine:

* Eye Open
* Eye Closed
* Blink Count

### Heart Rate Detection

The forehead region is selected as the Region of Interest (ROI).

Process:

```text
Face Detection
      ↓
Forehead ROI
      ↓
Green Channel Extraction
      ↓
Signal Processing
      ↓
Filtering
      ↓
Frequency Analysis
      ↓
Heart Rate (BPM)
```

---

## 📊 Output

The system displays:

* Live Webcam Feed
* Face Bounding Box
* Heart Rate (BPM)
* Blink Count
* Eye Status
* Real-Time Signal Graphs

Example:

```text
Heart Rate : 74 BPM

Blink Count : 15

Left Eye : Open

Right Eye : Open
```

---

## 🎯 Applications

* Health Monitoring
* Driver Drowsiness Detection
* Human-Computer Interaction
* Smart Healthcare Systems
* Research and Educational Projects

---

## 🔮 Future Enhancements

* Blood Oxygen (SpO2) Estimation
* Stress Detection
* Emotion Recognition
* Mobile Application Integration
* Cloud-Based Monitoring Dashboard

---

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a new branch
3. Commit changes
4. Push to your branch
5. Create a Pull Request

---

## 📜 License

This project is developed for educational and research purposes.

---

## 👩‍💻 Author

Navya Botla

B.Tech Project | Computer Vision | AI & Healthcare Applications
