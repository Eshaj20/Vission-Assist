# VisionAssist 🌙✨  
**AI-Powered Object Detection for Low-Light Environments**

[![YOLOv8](https://img.shields.io/badge/YOLOv8-00FFFF?style=flat)](https://ultralytics.com/yolov8)
[![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-C51A4A?logo=raspberrypi)](https://www.raspberrypi.com/)
[![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?logo=opencv)](https://opencv.org/)

<div align="center">
  <img src="https://github.com/Eshaj20/Vission-Assist/blob/master/video.mp4" alt="DemoVideo">
</div>

## 📌 Overview
-----------------------------------------------------------------------------------------------------------------------------------
VisionAssist is an intelligent navigation aid that detects objects in real-time under low-light conditions. Combining optimized YOLO models with affordable hardware, it provides:
- Real-time object detection (2-4 FPS on RPi 4)
- Distance and direction estimation
- Accessibility-focused feedback

## ✨ Key Features
--------------------------------------------------------------------------------------------------------------------------
| Feature | Description |
|---------|-------------|
| **Low-Light Vision** | Fine-tuned YOLOv8/YOLOv11 on ExDark dataset |
| **Spatial Mapping** | HC-SR04 ultrasonic sensor + SG90 servo |
| **Compact Design** | Raspberry Pi 4B with Pi Camera V2 |
| **Open-Source** | Fully customizable Python implementation |

🧰 Tech Stack
----------------------------------------------------------------------------------------------------------------------------------
AI Core
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch" height="20"> <img src="https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow" height="20">

Vision
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?logo=opencv" height="20"> <img src="https://img.shields.io/badge/Python-3776AB?logo=python" height="20">

Hardware
<img src="https://img.shields.io/badge/RPi.GPIO-A22846" height="20"> <img src="https://img.shields.io/badge/Picamera2-003366" height="20">

⚙️ Installation
---------------------------------------------------------------------------------------------------------------------------------------
# Clone with submodules
                git clone --recurse-submodules https://github.com/Eshaj20/VisionAssist.git

# Setup environment
                 cd VisionAssist
                 python -m venv venv
               source venv/bin/activate  # Linux/Mac
              # venv\Scripts\activate  # Windows

# Install dependencies
              pip install -r requirements.txt

🚀 Usage
-----------------------------------------------------------------------------------------------------

# Run with default settings
           python src/main.py

# Advanced options
             python src/main.py \
              --model yolov8n_custom.pt \
              --confidence 0.7 \
              --scan_angle 90

## 📊 Performance Benchmarks
-----------------------------------------------------------------------------------------------------------

### Model Comparison (ExDark Dataset)
| Metric        | YOLOv8 | YOLOv11 | Improvement |
|--------------|--------|---------|-------------|
| **mAP@0.5**  | 38%    | 42%     | ↑ 10.5%     |
| **Precision** | 0.81   | 0.83    | ↑ 2.5%      |
| **Recall**   | 0.74   | 0.78    | ↑ 5.4%      |


Hardware Benchmarks
--------------------------------------------------------------------------

             # Raspberry Pi 4B (4GB)
             Average Inference Time: 450ms ± 23ms
              Power Consumption: 3.2W @ 5V

 🔄 System Workflow

```mermaid
flowchart TD
    A[COCO Dataset] --> B[Object Detection Training]
    C[ExDark Dataset] --> B
    D[Face Dataset] --> E[Face Recognition Training]
    
    B --> F[ML Model]
    E --> F
    
    F --> G[Raspberry Pi 3B]
    H[Camera Module] --> G
    I[Ultrasonic Sensor] --> G
    J[Servo Motor] --> G
    
    G --> K[Object Detection]
    G --> L[Face Recognition]
    G --> M[Distance Calculation]
    G --> N[Direction Calculation]
    
    K --> O[Audio Output]
    L --> O
    M --> O
    N --> O
    
    O --> P["Output: Object Name, Face ID, Distance, Direction"]
