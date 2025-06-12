# 🚗 Car Detection System

A robust computer vision system for vehicle detection, license plate recognition (with Arabic support), speed estimation, and driving behavior analysis—specifically tailored for Tunisian traffic surveillance.

---

## 📌 Overview

This project integrates state-of-the-art deep learning techniques and computer vision tools to analyze traffic videos. It can:
- Detect and track vehicles in real-time.
- Recognize license plates, including Arabic text.
- Estimate vehicle speed from video footage.
- Analyze driver behavior for safety monitoring.
- Collect and preprocess vehicle data from the Tunisian marketplace **Tayara.tn**.

---

## ✨ Key Features

### 🚘 Vehicle Detection & Tracking
- Real-time detection using YOLOv8.
- Multi-object tracking with ByteTrack.
- Unique vehicle ID assignment across frames.
- Speed calculation using frame-difference analysis.

### 🔠 License Plate Recognition
- Automatic license plate detection.
- Arabic and English OCR using EasyOCR.
- Support for Tunisian plate formats.
- Custom-trained model for high precision.

### 🧠 Driving Behavior Classification
- Person detection within vehicles.
- Classifies driver behavior (e.g., phone usage, seatbelt detection).
- Real-time behavior flagging.

### 🧹 Data Collection & Processing
- Web scraping of Tunisian car listings via Tayara.tn.
- Automated image download & high-res enhancement.
- Clean dataset preparation for training models.

---

## 🧰 Tech Stack

| Area              | Tools & Libraries                       |
|-------------------|------------------------------------------|
| **Detection**     | Ultralytics YOLOv8, OpenCV               |
| **OCR**           | EasyOCR (Arabic + English)               |
| **ML Framework**  | PyTorch                                  |
| **Web Scraping**  | Selenium                                 |
| **Data Handling** | NumPy, Pandas                            |
| **Visualization** | Matplotlib, Pillow                       |

---

## 🧠 Models

| Model Type               | File Name                | Description                            |
|--------------------------|--------------------------|----------------------------------------|
| Vehicle Detection        | `yolov8x.pt`             | YOLOv8 for real-time car detection     |
| License Plate Detection  | `plate_detection.pt`     | Custom YOLO model for plate detection  |
| Driving Behavior         | `yolo_classification.pt` | Detects unsafe driver behavior         |

---

## ⚙️ Installation

### ✅ Prerequisites
- Python 3.8+
- CUDA-compatible GPU (optional but recommended)
- Git

### 📦 Install Dependencies

```bash
pip install -r requirements.txt
