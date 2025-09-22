# Project 1: CIFAR-10 Image Classification

## Overview
This project demonstrates the PyTorch workflow for computer vision tasks using the **CIFAR-10 dataset**.  
We implemented and compared two architectures:
1. **Feedforward Neural Network (FCNN)** – baseline, ~45% accuracy
2. **Convolutional Neural Network (CNN)** – improved accuracy up to ~81%

## Key Findings
- CNN outperformed FCNN by 35 percentage points.
- Data augmentation (rotation, flips) improved generalisation.
- Class-wise accuracy: strong on ships (90.5%), weaker on cats (58.2%).

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook project1_code.ipynb
