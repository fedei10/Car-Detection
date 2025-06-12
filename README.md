# Car-Detection



# Car Detection System - GitHub README

Based on my analysis of the repository, here's a comprehensive GitHub README for your Car Detection project:

```markdown
# Car Detection System

A comprehensive computer vision system for vehicle detection, license plate recognition, and driving behavior analysis, specifically designed for Tunisian traffic monitoring.

## Overview

This project implements an advanced car detection system that combines multiple AI models to analyze traffic videos and images. The system can detect vehicles, recognize license plates (including Arabic text), calculate vehicle speeds, and classify driving behaviors.

## Features

### 🚗 Vehicle Detection & Tracking
- Real-time vehicle detection using YOLO models
- Multi-object tracking with ByteTrack
- Speed calculation and monitoring
- Vehicle ID assignment and persistence

### 🔤 License Plate Recognition
- Automatic license plate detection
- OCR text extraction using EasyOCR
- Support for Arabic and English text
- Tunisian license plate format recognition

### 👤 Driving Behavior Analysis
- Safe driving behavior classification
- Person detection within vehicles
- Real-time behavioral assessment

### 📊 Data Collection Pipeline
- Web scraping from Tayara.tn marketplace
- Automated image downloading and processing
- Data preprocessing for model training

## Technical Stack

- **Computer Vision**: OpenCV, Ultralytics YOLO
- **OCR**: EasyOCR with Arabic language support
- **Machine Learning**: PyTorch, Custom YOLO models
- **Data Processing**: NumPy, Pandas
- **Web Scraping**: Selenium WebDriver
- **Image Processing**: Pillow, Matplotlib

## Models Used

The system utilizes multiple specialized models:
- **Vehicle Detection**: YOLO11x for general vehicle detection
- **License Plate Detection**: Custom trained model (`plate_detection.pt`)
- **Driving Behavior**: Custom classification model (`yolo_classification.pt`)

## Installation

### Prerequisites
- Python 3.8+
- CUDA-compatible GPU (recommended)
- Git

### Required Dependencies
```bash
pip install ultralytics
pip install opencv-python
pip install easyocr
pip install Pillow
pip install numpy
pip install pandas
pip install selenium
pip install matplotlib
```

## Usage

### 1. Data Collection
Run the scraping notebooks to collect training data:
- `tayara_scraping.ipynb` - Scrape vehicle listings
- `tayara_ImageDownload.ipynb` - Download vehicle images

### 2. Video Processing
Use the main workflow for video analysis:
- `workflow (1).ipynb` - Complete detection pipeline

### Key Functions

#### Vehicle Detection and Tracking
The system processes video frames to detect and track vehicles with unique IDs.

#### License Plate Recognition
Specialized OCR processing for Tunisian license plates with Arabic text support.

#### Speed Calculation
Real-time speed estimation based on vehicle movement between frames.

## Configuration

### Model Paths
Configure your model paths in the notebook:
- Plate detection model: `models/plate_detection.pt`
- Safe driving model: `models/yolo_classification.pt`

### Video Input
Set your video path for processing:
- Supported formats: MP4, AVI, MOV
- Recommended: 30 FPS for accurate speed calculation

## Features in Detail

### Arabic Text Support
The system includes specialized handling for Arabic license plates and can format text in the traditional Tunisian format.

### Multi-Modal Analysis
- **Visual Detection**: YOLO-based object detection
- **Text Recognition**: EasyOCR for license plate reading  
- **Behavioral Analysis**: Custom classification for driving patterns

### Performance Optimization
- Frame skipping for real-time processing
- GPU acceleration support
- Efficient memory management

## Data Pipeline

### Web Scraping Component
Automated data collection from Tayara.tn marketplace, extracting vehicle information and images for model training.

### Image Processing
High-resolution image downloading with URL modification for better quality training data.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Ultralytics for YOLO implementation
- EasyOCR team for Arabic OCR support
- OpenCV community for computer vision tools

## Contact

For questions and support, please open an issue in the GitHub repository.
```

This README is based on the comprehensive analysis of your codebase, which includes vehicle detection capabilities [1](#0-0) , license plate recognition with Arabic text support [2](#0-1) , speed calculation functionality [3](#0-2) , and a complete data collection pipeline through web scraping [4](#0-3)  and image downloading [5](#0-4) .

## Notes

The README reflects the multi-faceted nature of your project, which combines computer vision, OCR, and web scraping technologies. The system appears to be specifically designed for Tunisian traffic monitoring, with special attention to Arabic license plate recognition and local marketplace data collection from Tayara.tn. The modular structure with separate notebooks for different functionalities makes it easy for users to understand and contribute to specific components.
