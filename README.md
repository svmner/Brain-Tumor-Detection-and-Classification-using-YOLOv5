# Brain Tumor Detection and Classification using YOLOv5 🎯🧠

This repository contains the code and documentation for my B.Tech Practice School project at Manipal Institute of Technology, titled **"Brain Tumor Detection and Classification using YOLOv5"**. The project explores the use of deep learning and object detection—specifically YOLOv5—for real-time brain tumor detection and classification using MRI scans.

## 🧪 Problem Statement
Brain tumors are life-threatening and require early detection for effective treatment. Manual inspection of MRI scans by radiologists is time-consuming and error-prone due to inter-observer variability and fatigue. This project aims to develop a fast and accurate AI-based detection system to classify three major types of brain tumors:
- **Glioma**
- **Meningioma**
- **Pituitary Tumor**

## 💡 Objective
To build an optimized YOLOv5-based object detection model capable of:
- Accurately identifying and localizing tumors in MRI scans.
- Enhancing detection performance through architectural modifications.
- Ensuring practical deployment via improved speed-accuracy trade-off.

## 📂 Dataset
The dataset used for this project is the [**Medical Image Dataset: Brain Tumor Detection**](https://www.kaggle.com/datasets/pkdarabi/medical-image-dataset-brain-tumor-detection/data) made available via Kaggle. It contains:
- **3,903 MRI images** labeled with bounding boxes and class information.
- Four classes: **Glioma**, **Meningioma**, **Pituitary Tumor**, and **No Tumor**.
- All images were annotated with precise bounding boxes and later converted to YOLOv5-compatible format.

## 🧠 Methodology
- **Baseline Model**: YOLOv5s trained on the converted dataset.
- **Architecture Enhancements**: Incorporated Spatial Pyramid Pooling (SPP), Enhanced Spatial Attention (ESA), and Squeeze-and-Excitation (SE) modules.
- **Hyperparameter Tuning**: Conducted using the **Optuna** framework with Bayesian optimization.
- **Custom Evaluation Metric**: Introduced **Performance-Speed Ratio (PSR)** to evaluate detection accuracy vs inference speed.


## ⚙️ Tech Stack
- **Framework**: [YOLOv5 by Ultralytics](https://github.com/ultralytics/yolov5)
- **Language**: Python 3.11
- **Libraries**: PyTorch, OpenCV, NumPy, Optuna, Matplotlib
- **Hardware**: NVIDIA RTX 3060 GPU (12GB VRAM)

