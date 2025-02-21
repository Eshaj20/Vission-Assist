 VisionAssist – AI-Powered Object Detection for Low-Light Environments  🚀

📌 Overview

VisionAssist is an AI-based object detection system designed for low-light environments. It leverages YOLOv8 and YOLOv11 models, fine-tuned on the ExDark dataset, to accurately detect objects in challenging lighting conditions. The system integrates Raspberry Pi, ultrasonic sensors, and servo motors for real-time distance and direction estimation, enhancing accessibility and navigation assistance.

🔥 Features

✅ Low-Light Object Detection – Uses YOLOv8 & YOLOv11 fine-tuned on the ExDark dataset.✅ Real-Time Processing – Runs efficiently on Raspberry Pi with optimized deep-learning models.✅ Distance & Direction Estimation – Uses ultrasonic sensors & servo motors to provide object location feedback.✅ Hardware Integration – Seamless connection with sensors for a complete assistive solution.

   🛠 Hardware Components

🔹 Raspberry Pi – Runs the object detection model.
🔹 Ultrasonic Sensor – Measures object distance.
🔹 Servo Motor – Adjusts the sensor’s direction to scan the surroundings.

🖥 Software & Tools Used

🐍 Python – Core programming language.

🔍 YOLOv8 & YOLOv11 – Object detection models.

📸 OpenCV – Image processing and real-time video handling.

🧠 PyTorch/TensorFlow – Deep learning framework.

🌍 GitHub – Version control and project collaboration.


   ⚙ Installation & Setup

1️⃣ Clone the Repository

              git clone https://github.com/Eshaj20/VissionAssist.git
              cd VisionAssist

2️⃣ Install Dependencies

              pip install -r requirements.txt

3️⃣ Run the Object Detection Model

             python vision_assist.py



   🎯 Usage

🔹 Start the system – The camera captures real-time frames.🔹 Object Detection – The model detects objects and provides bounding boxes.🔹 Distance Estimation – The ultrasonic sensor measures object distance.🔹 Direction Assistance – Servo motors adjust angles for better coverage.

   📊 Results & Performance

![image](https://github.com/user-attachments/assets/44521981-4f45-40c9-8040-0e5420aca444)
📌 Mean Average Precision (mAP): 38% (Add actual performance metrics)📌 Precision: 0.81📌 Recall: 0.74

📌 Distance Measurement Accuracy:

![Screenshot 2025-02-21 184316](https://github.com/user-attachments/assets/0d8babf5-75ad-44fb-b3d9-b23a9f6c4bff)

🔹 Average Error (m): 0.062, 0.058, 0.072, 0.11, 0.16
🔹 Standard Deviation: 0.07, 0.06, 0.10, 0.12, 0.28

📌 Accuracy in Low-Light: 81.4% (Performance comparison before & after fine-tuning)

   🚀 Future Improvements

🔹 Edge AI Optimization – Improve real-time processing on Raspberry Pi.
🔹 Face Recognition Integration – (Previously attempted but faced hardware limitations.
)🔹 Voice Assistance – Convert detections into audio feedback for visually impaired users.

