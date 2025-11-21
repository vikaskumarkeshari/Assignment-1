# CIFAR-10 Image Classification Using Convolutional Neural Networks (CNN)

## Overview
This project implements an image classification model using a **Convolutional Neural Network (CNN)** on the **CIFAR-10 dataset** as part of **Assignment-1**.  
The objective is to select a dataset from Google Dataset Search and apply any machine-learning algorithm covered in class.

The CNN model achieves:

- **Training Accuracy:** 95%  
- **Testing Accuracy:** 96%

No normalization or data augmentation was used. The model was trained directly on raw pixel values.

---

## Dataset

**Name:** CIFAR-10  
**Source:** Google Dataset Search / Keras Datasets  

**Details:**
- 60,000 images (32×32 RGB)
- 10 classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck
- 50,000 training images
- 10,000 testing images

**Preprocessing:**
- Raw pixel values (0–255)  
- No normalization  
- No augmentation  

---

## Abstract
The CIFAR-10 dataset is widely used as a benchmark for evaluating image classification models.  
This project builds a CNN from scratch using Python to classify the dataset’s 10 image categories.  
Despite training on raw image pixel values without normalization or augmentation, the model achieves **96% test accuracy**, demonstrating strong performance and effective feature learning.

---

## Methodology

### Preprocessing
- Loaded dataset using Keras  
- Used raw 0–255 pixel values  
- One-hot encoded labels  
- No scaling  
- No augmentation  

### CNN Architecture
- Convolutional layers with ReLU activation  
- MaxPooling layers  
- Flatten layer  
- Dense layers  
- Softmax output layer (10 classes)

### Training
- **Optimizer:** Adam  
- **Loss:** Categorical Cross-Entropy  
- **Batch Size:** 32  
- **Epochs:** 20 (or configured)  
- **Metric:** Accuracy  

---

## Results

| Model | Training Accuracy | Testing Accuracy | Notes |
|-------|-------------------|------------------|-------|
| CNN (This Work) | 95% | 96% | No normalization, no augmentation |

Screenshots of training curves and predictions can be found in the `results/` folder.

---

## Repository Structure
