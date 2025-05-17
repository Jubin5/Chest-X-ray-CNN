# Chest X-ray Disease Prediction using CNN and Ensemble Learning

This project implements a deep learning pipeline for detecting chest diseases from X-ray images using Convolutional Neural Networks (CNNs). An ensemble of pre-trained models (VGG and ResNet) is used to improve performance and generalization.

## 🔍 Overview

Chest X-rays are one of the most common medical imaging techniques for diagnosing pulmonary diseases. This project aims to automate the classification of chest X-ray images using deep learning techniques, achieving a high diagnostic performance.

- **Model Architecture**: Custom CNN + Ensemble of VGG and ResNet
- **Accuracy Achieved**: 83.8%
- **Loss**: 0.37
- **Dataset**: Publicly available Chest X-ray dataset (Kaggle Chest X-ray Pneumonia dataset)

---

## 🧠 Methodology

### 1. **Data Preprocessing**
- Image resizing and normalization
- Data augmentation (flip, rotation, zoom)
- Train/validation/test split

### 2. **Model Architecture**
- Custom CNN for initial experiments
- Transfer learning using:
  - **VGG16**
  - **ResNet50**
- Ensemble learning by averaging model predictions or using a meta-classifier

### 3. **Training**
- Optimizer: Adam
- Loss Function: Binary Crossentropy / Categorical Crossentropy (depending on the dataset)
- Metrics: Accuracy, Precision, Recall
- Early stopping and learning rate reduction on plateau

---

## 📊 Results

| Model         | Accuracy | Loss |
|---------------|----------|------|
| CNN (baseline)| ~76%     | ~0.48|
| VGG16         | ~82%     | ~0.40|
| ResNet50      | ~81.5%   | ~0.42|
| **Ensemble**  | **83.8%**| **0.37** |

---

## 📁 Project Structure

