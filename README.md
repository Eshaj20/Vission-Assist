VisionAssist – AI-Powered Object Detection for Low-Light Environments

Overview

VisionAssist is an AI-based object detection system designed for low-light environments. It leverages YOLOv8 and YOLOv11 models, fine-tuned on the ExDark dataset, to accurately detect objects in challenging lighting conditions. The system integrates Raspberry Pi, ultrasonic sensors, and servo motors for real-time distance and direction estimation, enhancing accessibility and navigation assistance.

Features

Low-Light Object Detection – Uses YOLOv8 & YOLOv11 fine-tuned on ExDark dataset.

Real-Time Processing – Runs efficiently on Raspberry Pi with optimized deep-learning models.

Distance & Direction Estimation – Uses ultrasonic sensors & servo motors to provide object location feedback.

Hardware Integration – Seamless connection with sensors for a complete assistive solution.

Hardware Components

Raspberry Pi – Runs the object detection model.

Ultrasonic Sensor – Measures object distance.

Servo Motor – Adjusts the sensor’s direction to scan the surroundings.

Software & Tools Used

Python – Core programming language.

YOLOv8 & YOLOv11 – Object detection models.

OpenCV – Image processing and real-time video handling.

PyTorch/TensorFlow – Deep learning framework.

GitHub – Version control and project collaboration.

Installation & Setup

1. Clone the Repository

git clone https://github.com/Eshaj20/VissionAssist.git
cd VisionAssist

2. Install Dependencies

pip install -r requirements.txt

3. Run the Object Detection Model

python vision_assist.py

(Modify the filename if needed based on your project structure.)

Usage

Start the system – The camera captures real-time frames.

Object Detection – The model detects objects and provides bounding boxes.

Distance Estimation – The ultrasonic sensor measures object distance.

Direction Assistance – Servo motors adjust angles for better coverage.

Results & Performance

Mean Average Precision (mAP): 38% (Add actual performance metrics)
precision : 0.81
Recall : 0.74
![image](https://github.com/user-attachments/assets/f5126c69-ef87-4cc2-8d8d-58b7f3ae2599)

Distance Measurement Accuracy :
The system's distance estimation was evaluated, and the results are summarized below:
![Screenshot 2025-02-21 184316](https://github.com/user-attachments/assets/47e90436-17f4-4d76-a0d3-00c3c6eba2de)

Accuracy in Low-Light: 81.4% (Performance comparison before & after fine-tuning)

Future Improvements

Edge AI Optimization – Improve real-time processing on Raspberry Pi.

Face Recognition Integration – (Previously attempted but faced hardware limitations).

Voice Assistance – Convert detections into audio feedback for visually impaired users.
