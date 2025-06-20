# 🗑️ Garbage Classification using Deep Learning

This project aims to build a deep learning-based image classification model to automatically classify waste images into five categories: **cardboard**, **metal**, **paper**, **plastic**, and **white-glass**. The system is designed to support **automated waste segregation**, promoting smarter recycling and sustainable waste management.

---

## 📁 Dataset Description

The dataset used in this project is organized into five categories, each stored in its own folder. This format is compatible with image classification frameworks like TensorFlow/Keras (`flow_from_directory`) and PyTorch (`ImageFolder`).
dataset/
├── cardboard/ # Images of cardboard waste (e.g., boxes, packaging)
├── metal/ # Images of metallic waste (e.g., cans, foils)
├── paper/ # Images of paper waste (e.g., sheets, newspapers)
├── plastic/ # Images of plastic waste (e.g., bottles, wrappers)
└── white-glass/ # Images of white or transparent glass items


Each folder contains multiple images depicting the corresponding waste type. The dataset can be expanded for real-world scenarios and customized further for recycling applications.

---

## 🎯 Project Objective

- Build a robust deep learning model to classify garbage images
- Enable smart waste sorting using computer vision
- Reduce human labor in garbage segregation processes
- Lay groundwork for real-time embedded smart-bin deployment

---

## 🧠 Model Architecture

- **Base Model:** MobileNetV2 (pre-trained on ImageNet)
- **Custom Classification Head:**
  - AveragePooling2D
  - Flatten
  - Dense (ReLU) + Dropout
  - Final Dense layer with Softmax for multi-class prediction

### 🔧 Key Techniques

- **Transfer Learning**
- **Data Augmentation** (rotation, zoom, shift, flip)
- **Dropout Regularization**
- **Class Weighting** to handle imbalance
- **Adam Optimizer + Categorical Crossentropy**





