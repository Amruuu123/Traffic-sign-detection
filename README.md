# Traffic-sign-detection
# 🚦 Traffic Sign Detection using CNN and OpenCV

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green?logo=opencv)
![PyTorch](https://img.shields.io/badge/PyTorch-1.x-red?logo=pytorch)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

This project focuses on real-time **Traffic Sign Detection and Classification** using a CNN trained on the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset. It includes both model training and live detection using a webcam feed.

---

## 📦 Dataset

We use the **[German Traffic Sign Recognition Benchmark (GTSRB)](https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign)** from Kaggle.

- 43 classes of traffic signs
- 50,000+ labeled images
- Pre-split into train and test sets

---

## 📁 Project Structure

│
├── Untitled.ipynb # Jupyter Notebook for training the CNN
├── ho.py # Script for real-time traffic sign detection using webcam
├── model.pth # Saved trained model weights
├── class_names.csv # Mapping of class index to sign name
├── requirements.txt # Python dependencies
└── README.md # Project documentation

---

## 🧠 Model Overview

- Framework: PyTorch
- Architecture: Custom CNN (or ResNet-based)
- Output: 43-class softmax classifier
- Trained with: CrossEntropyLoss + Adam optimizer
- Evaluation: Accuracy, Confusion Matrix

---

## 🔧 Installation

1. **Clone the repository**
```bash
git clone https://github.com/your-username/traffic-sign-detection.git
cd traffic-sign-detection

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
