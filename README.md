# MNIST Digit Classification Using Convolutional Neural Networks (CNN)

## 📌 Overview
This project implements a Convolutional Neural Network (CNN) model for classifying handwritten digits from the MNIST dataset as part of **Assignment-1**.

The task was to:
- Select a dataset from Google Dataset Search  
- Apply any ML/DL algorithm covered in class  
- Implement using Python  
- Provide code, README, and a report  

The model achieves:

- **Training Accuracy:** 99.85%  
- **Testing Accuracy:** 98.00%

Simple normalization was used. No augmentation techniques were applied.

---

## 📊 Dataset

**Name:** MNIST – Handwritten Digit Dataset  
**Source:** Google Dataset Search / Keras Datasets  

### Dataset Details
- 70,000 grayscale images  
- Image size: **28×28**  
- 10 classes: digits **0–9**  
- 60,000 training images  
- 10,000 test images  

### Preprocessing
- Pixel values normalized **0–255 → 0–1**
- Reshaped to **(28, 28, 1)**  
- Labels kept in integer form → sparse classification  

---

## 📝 Abstract
The MNIST dataset is a widely used benchmark for image classification.  
This project builds a CNN using Python and TensorFlow/Keras to classify handwritten digits.

Despite the model’s simplicity and minimal preprocessing, it achieves excellent performance with **98% test accuracy**, showing strong feature extraction by the CNN.

---

## ⚙️ Methodology

### 1️⃣ Preprocessing
- Loaded dataset from Keras  
- Normalized pixel values to `[0, 1]`  
- Added channel dimension  
- Used sparse labels  

### 2️⃣ CNN Architecture
The CNN contains the following layers:

- `Conv2D(32 filters, 3×3, ReLU)`
- `MaxPooling2D(2×2)`
- `Flatten()`
- `Dense(100, ReLU)`
- `Dense(10, Softmax)`

This architecture is ideal for MNIST due to its simplicity and high performance.

### 3️⃣ Training
- **Optimizer:** SGD (momentum=0.9)  
- **Loss:** Sparse Categorical Cross-Entropy  
- **Batch Size:** 32  
- **Epochs:** 10  
- **Metric:** Accuracy  

---

## ✅ Results

| Model | Training Accuracy | Testing Accuracy | Notes |
|-------|------------------|------------------|-------|
| CNN (This Work) | **99.85%** | **98.00%** | Simple CNN, normalized pixels |

Plots for accuracy, loss, and the confusion matrix are available in the `results/` folder.

---

## 📷 Output Visualizations
The project includes:

- Training Accuracy Curve  
- Training Loss Curve  
- Confusion Matrix  
- Classification Report  
- Sample Predictions  

All outputs are saved inside the **results/** directory.

---

## 📁 Repository Structure
