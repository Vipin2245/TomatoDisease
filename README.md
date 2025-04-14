# Tomato Leaf Disease Classification

A deep learning-based image classification system to detect **tomato leaf diseases** using Convolutional Neural Networks (CNNs) and Transfer Learning. This model can help farmers and agricultural professionals detect diseases early and take necessary actions to protect crop health.

---

## Problem Statement

Tomato plants are highly susceptible to various diseases that affect both the yield and quality of produce. Manual detection is time-consuming and error-prone, especially for large-scale farming. Early and accurate diagnosis is essential to prevent the spread of diseases and minimize crop losses.

**Goal:**  
Build an AI-powered image classification model that can automatically identify tomato leaf diseases with high accuracy from images.

---

## My Approach

To tackle this problem, I followed a structured pipeline:

### 1. **Data Collection & Preparation**
- Used the **PlantVillage** dataset from Kaggle containing 11 tomato leaf categories (including "healthy").
- Organized data into training and testing directories.
- Performed data augmentation using `ImageDataGenerator` to improve model generalization.

### 2. **Model Selection**
Implemented and compared multiple models:
- **Custom CNN**: Designed a simple CNN from scratch to establish a baseline.
- **Transfer Learning Models**:
  - **VGG16**
  - **InceptionV3**
  - **ResNet50**

### 3. **Training & Evaluation**
- Trained each model and monitored accuracy and loss over epochs.
- Evaluated using:
  - Classification reports
  - Confusion matrices
  - Accuracy/Loss curves

### 4. **Result Comparison**
Compared the performance of different models to choose the best one for future deployment.

---

## Dataset

- **Source**: [PlantVillage Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)
- Contains labeled images of tomato leaves across 11 classes (10 disease types + 1 healthy class).

---

## Model Performance

| Model       | Accuracy |
|-------------|----------|
| VGG16       | 97%      |
| InceptionV3 | 95%      |
| ResNet50    | 93%      |

> VGG16 outperformed others and is the best candidate for deployment.

---
