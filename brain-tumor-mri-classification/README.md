# Brain Tumor MRI Classification using CNN & EfficientNetB0

This repository contains the deep learning model and image processing pipeline developed for brain tumor classification using MRI scans as part of graduation project work.

## Overview
The project classifies brain MRI images into four distinct categories:
1. **Glioma Tumor**
2. **Meningioma Tumor**
3. **Pituitary Tumor**
4. **No Tumor**

## Dataset
The model was trained and evaluated using the publicly available dataset from Kaggle:
* **Dataset Link:** [Brain Tumor Classification (MRI) on Kaggle](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri)

## Architecture & Approach
* **Transfer Learning:** Utilizes **EfficientNetB0** pre-trained on ImageNet as the backbone feature extractor.
* **Data Processing & Augmentation:** Uses OpenCV for image reading and resizing (150x150), alongside robust data shuffling and splitting.
* **Optimization & Callbacks:** Implements ModelCheckpoint, TensorBoard, and ReduceLROnPlateau to optimize training and prevent overfitting.
* **Evaluation Metrics:** Evaluated using accuracy/loss curves, detailed classification reports, and Confusion Matrix heatmaps.
* **Model Deployment:** Includes script implementation to convert the trained model into TensorFlow Lite (`.tflite`) format for lightweight edge/mobile deployment.

## Requirements
Install the required dependencies using pip:
```bash
pip install -r requirements.txt