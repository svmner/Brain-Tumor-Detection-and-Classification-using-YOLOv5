# 🧠 Brain Tumor Detection Using YOLOv5

This repository presents a deep learning-based object detection model for identifying and localizing brain tumors from MRI scans using an enhanced YOLOv5 architecture. The project focuses on classifying three tumor types—**glioma**, **meningioma**, and **pituitary tumor**—using high-resolution annotated MRI images.

## 🚀 Overview

The model is built on YOLOv5s and incorporates:
- 🔲 **SPP (Spatial Pyramid Pooling)** for multi-scale feature representation
- 🎯 **ESA (Enhanced Spatial Attention)** for spatial region focus
- 📦 **SE (Squeeze-and-Excitation)** for channel-wise recalibration
- 🔧 **Hyperparameter tuning with Optuna (Bayesian Optimization)**

The final model achieves:
- **mAP@0.5:** `0.934`
- **Precision:** `0.924`
- **Recall:** `0.883`
- **Inference speed:** ~8.4 ms/image

📊 Dataset
Name: Medical Image Dataset - Brain Tumor Detection

Source: Kaggle Dataset by pkdarabi

Size: ~3,900 images

Modality: T1-weighted MRI scans

Classes:

0 – Glioma

1 – Meningioma

2 – Pituitary Tumor

3 – No Tumor

Label Format: Converted from YOLOv8 to YOLOv5 (.txt with normalized bounding boxes)

⚙️ Setup Instructions
Clone the repo

bash
Copy
Edit
git clone https://github.com/your-username/brain-tumor-detection-yolov5.git
cd brain-tumor-detection-yolov5
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Run training

bash
Copy
Edit
python train.py --img 640 --batch 16 --epochs 100 --data dataset.yaml --cfg yolov5s_spp_esa_se.yaml --weights yolov5s.pt
Evaluate model

bash
Copy
Edit
python val.py --weights runs/train/exp/weights/best.pt --data dataset.yaml
🧪 Tools & Frameworks
Python 3.10

PyTorch

YOLOv5 (Ultralytics v7.0)

Optuna

OpenCV, NumPy, Roboflow, Matplotlib
