# finalyear-project
Based on your uploaded project report titled **"Touchless Heartbeat Measurement Using Facial Video"**, here is a sample **README file** along with the **tools and technologies used**:

---

## 📄 README.md

### 📌 Project Title

**Touchless Heartbeat Measurement Using Facial Video**

---

### 🧠 Overview

This project implements a **non-invasive system** to measure heart rate using only facial video input from a webcam. It leverages **computer vision** and **signal processing** to estimate heartbeats in real-time, without any physical contact—ideal for healthcare, fitness, and telemedicine.

---

### 🎯 Objectives

* Estimate heart rate from facial videos using RGB signal analysis.
* Provide a real-time graphical interface (Tkinter GUI / Flask Web App).
* Alert users when heart rate exceeds a safe threshold (e.g., >90 BPM).
* Transmit live data using MQTT for remote health monitoring.

---

### ⚙️ Tools and Technologies Used

| Category          | Tools/Technologies                                        |
| ----------------- | --------------------------------------------------------- |
| Programming       | Python                                                    |
| Libraries         | OpenCV, NumPy, Pandas, Matplotlib, SciPy, Seaborn         |
| Signal Processing | FFT, ICA, EVM (Eulerian Video Magnification)              |
| Machine Learning  | (Optional) CNNs, SVM, TensorFlow, PyTorch                 |
| GUI               | Tkinter (Desktop GUI), Flask (Web Interface)              |
| IoT               | MQTT (Paho-MQTT Client, EMQX Broker)                      |
| Alert System      | Winsound (for buzzer sound on abnormal BPM)               |
| Hardware          | RGB Webcam (e.g., Logitech C920), Raspberry Pi (optional) |
| Development Tools | Jupyter Notebook, GitHub, Git                             |

---

### 🏗️ Features

* **Touchless pulse monitoring** via webcam.
* **Real-time BPM calculation** using FFT.
* **Live alerts** via sound and MQTT messaging.
* Dual interface: Web (Flask) & Desktop App (Tkinter).
* Designed for **low-cost hardware**.

---

📁 Project Structure
graphql
Copy
Edit
project-folder/
├── app.py                 # Flask web app for video streaming and alerts
├── touchless_hB3.py       # Tkinter-based GUI for heart rate detection and graph
├── templates/
│   ├── home.html
│   ├── detection.html
│   └── contact.html
├── static/
│   └── images/            # Heart & health visuals
├── TLHB.png               # Project banner or logo
├── README.md              # This file
🚀 How to Run
🖥️ Option 1: GUI Mode
bash
Copy
Edit
python touchless_hB3.py
🌐 Option 2: Web Mode (Flask)
bash
Copy
Edit
python app.py
Access in browser at: http://localhost:5000

🔊 Alert System
If BPM > 90: Red alert text is displayed, and a buzzer sound is triggered.

MQTT publishes:

heartbeat/count → Numerical BPM

heartbeat/status → "Normal Heartbeat" / "High Heartbeat"

📡 MQTT Setup
Broker: broker.emqx.io

You can monitor topics via MQTTX or similar tools.

📸 Sample Visuals Used
ECG waveform

Heart health graphics

Medical equipment illustrations
(See TLHB.png and supporting image assets.)

### 📊 Applications

* Telemedicine and remote health monitoring
* Fitness and sports monitoring
* Contactless monitoring in contagious environments (e.g., COVID wards)


### 👨‍💻 Contributors

* Shivansh Gupta
* Sarthak Gupta
* Sakshi Jain
  (Under the guidance of Prof. P.S. Sajjanshetti)

