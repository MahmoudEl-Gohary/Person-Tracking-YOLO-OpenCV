# Person Tracking and Route Visualization System

A computer vision system that tracks individual persons across video sequences and visualizes their movement paths using YOLOv8 object detection and OpenCV. Developed for DSAI 352 - Computer Vision course.

## 🎯 Project Overview

This Software enables the automatic detection, tracking, and visualization of routes for specific individuals in video footage. Users can interactively select a person from the first frame, and the system will track their movement throughout the entire video, generating a comprehensive route visualization.

## ✨ Key Features

- **Interactive Person Selection**: Visual interface for selecting the target person from detected individuals
- **Real-time Object Detection**: Utilizes YOLOv8 for accurate person detection
- **Tracking Algorithm**: Distance-based tracking with confidence scoring
- **Visualization**: Generates video output with tracked movement path overlay
- **Progress Monitoring**: Real-time processing progress indicators
- **GPU Optimization**: CUDA support for accelerated inference

## 🏗️ System Architecture

### Core Components

1. **YOLO Model Integration**: Pre-trained YOLOv8 nano model for person detection
2. **Video Processing Pipeline**: Frame-by-frame analysis with OpenCV
3. **Tracking Algorithm**: Center-point based tracking with distance thresholding
4. **Visualization Engine**: Route overlay and bounding box rendering
5. **Interactive Interface**: Matplotlib-based person selection

### Processing Workflow

```
Input Video → Frame Extraction → Person Detection → User Selection → 
Tracking Loop → Route Recording → Visualization → Output Video
```

## 🛠️ Technologies Used

- **Python 3.8+**
- **YOLOv8 (Ultralytics)** - Object detection framework
- **OpenCV** - Computer vision and video processing
- **PyTorch** - Deep learning backend
- **NumPy** - Numerical computations
- **Matplotlib** - Interactive visualization
- **IPython** - Enhanced display capabilities

## 📁 Project Structure

```
├── Proj.ipynb                    # Main implementation notebook
└── README.md                     # Project documentation
```

## 🚀 Getting Started

### Prerequisites

```bash
pip install ultralytics opencv-python torch numpy matplotlib ipython
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/person-tracking-yolo-opencv.git
cd person-tracking-yolo-opencv
```

2. Download YOLOv8 model (automatic on first run):
```python
from ultralytics import YOLO
model = YOLO('yolov8n.pt')  # Downloads automatically
```

### Quick Start

```python
# Run the complete tracking pipeline
output_video = main("path/to/your/video.mp4")
```

## 📝 Course Information

**Course**: DSAI 352 - Computer Vision  
**Institution**: University of science and technology at zewailcity
**Semester**: Spring 2025  
**Project Type**: Individual
## 📄 License

This project is created for educational purposes as part of coursework requirements.

---

*This project demonstrates practical application of computer vision techniques including object detection, tracking algorithms, and video processing for real-world surveillance and monitoring applications.*
