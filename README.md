# 🧥 Fashion MNIST Image Classification with CNN & Data Augmentation

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

This project implements a Convolutional Neural Network (CNN) to classify images from the **Fashion MNIST** dataset. To improve the model's generalization capability and reduce overfitting, **Data Augmentation** techniques are applied during the training process.

## 📌 Project Overview

The goal of this project is to accurately categorize clothing items into 10 distinct classes using Deep Learning.

- **Dataset:** Fashion MNIST (60,000 training images, 10,000 test images).
- **Image Shape:** 28x28 grayscale.
- **Model Architecture:** Sequential CNN with Dropout layers.
- **Technique:** Real-time Data Augmentation (Rotation, Shift, Zoom).
- **Test Accuracy:** **~87.65%**

## 📂 Dataset Classes

The dataset consists of the following labels:
0. T-shirt/top
1. Trouser
2. Pullover
3. Dress
4. Coat
5. Sandal
6. Shirt
7. Sneaker
8. Bag
9. Ankle boot

## 🧠 Model Architecture

The model is built using `tensorflow.keras` with the following structure:

1.  **Conv2D (32 filters)** + ReLU + MaxPooling2D + Dropout (0.2)
2.  **Conv2D (64 filters)** + ReLU + MaxPooling2D + Dropout (0.25)
3.  **Flatten Layer**
4.  **Dense (128 units)** + ReLU + Dropout (0.5)
5.  **Output Layer (10 units)** + Softmax

### 🔄 Data Augmentation Strategy
To make the model more robust, the following transformations were applied to the training data:
* **Rotation Range:** 10 degrees
* **Width Shift:** 10%
* **Height Shift:** 10%
* **Zoom Range:** 10%

## 📊 Results

The model was trained for **10 epochs**.

| Metric | Score |
| :--- | :--- |
| **Training Accuracy** | ~84% |
| **Validation Accuracy** | ~88% |
| **Test Accuracy** | **87.65%** |

> *Note: Data augmentation helped bridge the gap between training and validation accuracy, effectively reducing overfitting.*

## 📈 Visualizations

<img width="1001" height="393" alt="__results___15_0" src="https://github.com/user-attachments/assets/d933af36-de85-4eaf-a14d-b48bb3e1866f" />


