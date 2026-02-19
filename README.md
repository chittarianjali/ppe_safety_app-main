
# 🦺 Lightweight Multi-PPE Detection for Edge-Based Industrial Safety Monitoring

A real-time Personal Protective Equipment (PPE) detection system built using **YOLOv8** and deployed through a **Flask-based web application**. The system is designed for industrial environments to ensure worker safety compliance by detecting essential protective equipment such as helmets, safety vests, and boots along with person detection.

---

## 📌 Project Overview

Industrial environments require strict adherence to safety standards to prevent accidents and injuries. Manual supervision of PPE compliance is time-consuming, inconsistent, and prone to human error.

This project presents a lightweight deep learning-based framework that automatically detects multiple PPE components in real time using computer vision techniques. The system leverages YOLOv8 for high-speed object detection and integrates a Flask-based web interface for user-friendly deployment.

The solution is optimized for:

* Multi-class PPE detection
* Real-time monitoring
* Low-latency inference
* Edge-based industrial deployment

---

## 🚀 Features

* 🔍 Multi-class PPE detection
* 🎯 YOLOv8-based object detection model
* 📊 Performance evaluation using Precision, Recall, F1-score, and mAP
* 📸 Image upload detection
* 🎥 Real-time webcam detection
* 🌐 Flask-based web deployment
* ⚡ Lightweight architecture suitable for edge devices
* 📦 Easy scalability for industrial safety systems

---

## 🧠 Detected Classes

The model detects the following 4 classes:

* **Person**
* **Helmet**
* **Vest**
* **Boots**

---

## 🏗 System Architecture

The system follows a structured pipeline:

### 1️⃣ Dataset Preparation

* PPE Dataset for Workplace Safety (Roboflow)
* Bounding box annotations
* Multi-class object detection format compatible with YOLO

### 2️⃣ Model Training

* Pretrained YOLOv8 model fine-tuned on the PPE dataset
* Anchor-free detection mechanism
* Multi-scale feature extraction
* Optimized using SGD
* Loss Functions:

  * Bounding Box Loss
  * Classification Loss
  * Distribution Focal Loss

### 3️⃣ Model Deployment

* Trained weights integrated into Flask backend
* Image and webcam input processing
* Real-time inference with bounding boxes and confidence scores

---

## 📊 Model Performance

* **mAP@0.5:** 0.961
* **Best F1-Score:** 0.91 at confidence threshold 0.437
* High precision at higher confidence thresholds
* Strong recall at lower thresholds
* Reliable multi-person detection in complex industrial scenes

---

## 🖥 Web Application Modules

The deployed web interface includes:

* **Image Upload Module** – Upload static images for PPE detection
* **Webcam Module** – Real-time PPE detection
* **Detection Engine** – YOLOv8 inference backend
* **Output Visualization** – Annotated bounding boxes with confidence scores

---

## 🛠 Tech Stack

* Python
* YOLOv8 (Ultralytics)
* OpenCV
* Flask
* Roboflow Dataset
* NumPy
* Matplotlib

---

## 📂 Project Structure

```
├── app.py                  # Flask application
├── model/
│   └── best.pt              # Trained YOLOv8 weights
├── static/
│   └── uploads/             # Uploaded images
├── templates/
│   └── index.html           # Web interface
├── requirements.txt
└── README.md
```

---

## ⚙ Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/multi-ppe-detection.git
cd multi-ppe-detection
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run Application

```bash
python app.py
```

Then open:

```
http://127.0.0.1:5000/
```

---

## 🎯 Applications

* Industrial safety monitoring
* Construction site compliance
* Manufacturing plant supervision
* Automated workplace auditing
* Edge-based surveillance systems

---

## 📈 Future Improvements

* PPE violation alert system
* Real-time video stream processing
* Worker-level PPE compliance tracking
* Edge device optimization (Raspberry Pi / Jetson Nano)
* Integration with IoT-based safety systems

---


* Or make it look more attractive like a professional open-source project 🚀
