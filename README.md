# YOLOv8 Autonomous Driving Object Detection
This repository contains code and data for optimizing YOLOv8 small model for object detection and tracking, focused on autonomous driving applications. Includes methodology, results, and future improvements.

<br />

## 🌱 Introduction
This project was completed by Agnes Song as part of the Capstone Project in UCONN Master's program. It focuses on optimizing the YOLOv8 object detection model for applications in autonomous driving. The primary goal was to enhance the model's performance in detecting and tracking objects in dynamic and complex driving environments. Various techniques, including layer freezing, data augmentation strategies, advanced loss functions, and alternative optimizers, were explored. The final models were validated using metrics like mAP@50, precision, and real-world inference scenarios to assess their robustness and applicability for real-time deployment in autonomous systems

<br />

## 📍 Objective
This project focuses on optimizing the YOLOv8 small model for object detection and tracking in autonomous driving scenarios. The goal was to improve model accuracy and robustness while maintaining real-time performance for deployment in dynamic environments.  

<br />

## 🛠️ Methodology  
- **Model Configurations:** Evaluated 8 different configurations to identify the best-performing setup.  
- **Techniques Applied:**  
  - Layer freezing
  - Data augmentation
  - Advanced loss functions
- **Validation:**  
  - Conducted video inference and multi-object tracking experiments.  

<br />

## Project Structure 
```
yolov8-autonomous-driving/
│   README.md
│   LICENSE
├── data/ # dataset, annotations, and yaml files
├── notebook/ # training, inference, and evaluation scripts
└── results/ # metrics, plots, and video results
```

Scripts:
- 01-coco-data-preparation.ipynb - data preprocessing, annotation formatting, handle data imbalancing, etc.
- 02-yolov8-model-training-a100.ipynb - configure/train model
- 03-yolov8-results-analysis.ipynb - evaluate model performance and generate visualizations for analysis
- 04-video-inference.ipynb - apply the trained model for video inference

<br />

## 📊 Results
- Achieved an **8% improvement in mAP@50**, with a final score of 0.785.  
- The model demonstrated strong detection and tracking capabilities in most scenarios, but challenges like handling occlusion and complex scenes remain.

<br />

## 💭 Future Improvements
Future improvements on this project would include:
- further refine the model to handle occlusions and crowded environments
- integrate additional real-world testing datasets for enhanced robustness
