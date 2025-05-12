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

## 📊 Dataset

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

