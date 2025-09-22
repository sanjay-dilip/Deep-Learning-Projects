# Project 1: CIFAR-10 Image Classification with PyTorch

## 📌 Overview
This project implements and compares two deep learning models for image classification on the **CIFAR-10 dataset**:
1. A baseline **Feedforward Neural Network (FCNN)**
2. A **Convolutional Neural Network (CNN)**

The goal is to understand how different architectures handle image data and to evaluate their performance.

---

## 📊 Dataset
- **CIFAR-10**: 60,000 color images (32x32 pixels) across 10 classes.
- Split: 50,000 training + 10,000 test samples.
- Classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck.

---

## ⚙️ Methodology
- Data preprocessing with normalization and augmentation (random rotations, flips).
- Implemented FCNN and CNN architectures in **PyTorch**.
- Training with Adam optimizer + CrossEntropy loss.
- Evaluation using:
  - Accuracy curves
  - Confusion matrix
  - Per-class accuracy
  - Classification report

---

## 🚀 Results
- **FCNN Accuracy**: ~45% (underfits due to lack of spatial awareness)
- **CNN Accuracy**: ~81% (captures spatial features effectively)
- CNN achieved a **35 percentage point improvement** over the baseline.
- Strong class-wise performance on `ship` (90.5%) and weaker on `cat` (58.2%).

---

## 📂 Files
- `cifar10_image_classification_pytorch_clean.ipynb` – Clean notebook (no outputs).
- `cifar10_image_classification_pytorch.html` – Static HTML viewer.
- (Optional) `cifar10_cnn_model.pth` – Saved trained model.

---

## ▶️ How to Run
```bash
pip install -r ../requirements.txt
jupyter notebook cifar10_image_classification_pytorch.ipynb
