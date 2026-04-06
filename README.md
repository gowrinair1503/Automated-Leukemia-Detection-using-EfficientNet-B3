Automated Leukemia Detection using EfficientNet-B3
Overview

This project presents an automated system for detecting leukemia from microscopic blood smear images using deep learning. The model leverages EfficientNet-B3, a state-of-the-art convolutional neural network, to classify images into:

Leukemia (ALL)
Normal (HEM)

The goal is to assist medical professionals by reducing manual effort, improving diagnostic accuracy, and enabling early detection.

Problem Statement

Traditional leukemia detection:

Is time-consuming
Requires expert hematologists
Is prone to human error

This project addresses these challenges by building an AI-based automated detection system.

Objectives
Develop an automated leukemia detection system
Use EfficientNet-B3 for image classification
Train the model on the C-NMC dataset
Improve accuracy and reduce diagnosis time
Assist doctors in decision-making
Dataset
Dataset Name: C-NMC (Classification of Normal vs Malignant Cells)
Total Images: 10,000+ (used subset: 4200 images)
Classes:
ALL (Leukemia cells)
HEM (Normal cells)
High-resolution microscopic blood smear images
System Architecture
Input blood smear images
Image preprocessing (resize and normalization)
Dataset split (70% training, 30% testing)
Feature extraction using EfficientNet-B3
Classification (Normal or Leukemia)
Performance evaluation
Methodology
Used transfer learning with EfficientNet-B3 (pretrained on ImageNet)
Applied preprocessing:
Image resizing (300×300)
Normalization
Data augmentation (rotation, zoom, flipping)
Frozen base layers initially and fine-tuned top layers
Used:
Optimizer: Adam
Learning Rate: 1e-5
Loss Function: Binary Crossentropy
Modules
Dataset Collection and Preparation
Data Preprocessing
Dataset Splitting
Feature Extraction
Model Training
Model Evaluation
Prediction System
Technologies Used
Programming Language: Python
Frameworks: TensorFlow, Keras
Tools:
Google Colab
Jupyter Notebook / VS Code
Requirements
Software
Python 3.8+
TensorFlow / Keras
OpenCV, NumPy, Matplotlib
Hardware
Intel i5/i7 or higher
Minimum 8 GB RAM (16 GB recommended)
GPU (optional but recommended)
Results
Training Accuracy: ~75.67%
Test Accuracy: ~75.83%
Minimal overfitting

Some misclassifications occur due to similarities in cell morphology and variations in image quality.
