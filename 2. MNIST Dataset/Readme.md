# ✍️ Handwritten Digit Classification using Artificial Neural Networks (ANN)

## 🔍 Project Overview
This project focuses on classifying handwritten digits (0–9) using the **MNIST dataset** and an **Artificial Neural Network (ANN)**.  
The model learns pixel-level patterns from grayscale images to accurately recognize handwritten numbers.

The project demonstrates a complete deep learning pipeline including data preprocessing, ANN model building, training, evaluation, and visualization.

---

## 🧠 Problem Statement
Build a classification model that can correctly identify handwritten digits (0–9) from 28×28 grayscale images.

**Target Classes:**  
Digits from `0` to `9`

---

## 🗂️ Dataset Information
- **Dataset:** MNIST Handwritten Digits Dataset
- **Source:** TensorFlow / Keras built-in dataset
- **Training Samples:** 60,000 images
- **Test Samples:** 10,000 images
- **Image Size:** 28 × 28 pixels
- **Problem Type:** Multi-class Classification

---

## 🛠️ Technologies & Tools
- **Programming Language:** Python  
- **Libraries:** NumPy, Matplotlib  
- **Machine Learning Utilities:** Scikit-learn  
- **Deep Learning Framework:** TensorFlow, Keras  

---

## 🔄 Project Workflow

### 1️⃣ Data Loading
- Loaded MNIST dataset directly from Keras
- Separated training and testing datasets

---

### 2️⃣ Data Preprocessing
- Normalized pixel values to range `[0, 1]`
- Flattened 28×28 images into 1D vectors
- Converted class labels for multi-class classification

---

### 3️⃣ Model Building (ANN)
- Built a Sequential Artificial Neural Network
- Architecture includes:
  - Flatten layer
  - Dense hidden layers with **ReLU activation**
  - Output layer with **Softmax activation**
- Designed for 10-class classification

---

### 4️⃣ Model Compilation
- **Loss Function:** Sparse Categorical Crossentropy  
- **Optimizer:** Adam  
- **Metric:** Accuracy  

---

### 5️⃣ Model Training
- Trained the model for **10 epochs**
- Used **validation split** to monitor generalization
- Stored training history for visualization

---

### 6️⃣ Model Evaluation
- Evaluated performance on unseen test data
- Generated predictions for handwritten digit images

---

### 7️⃣ Performance Visualization
- Training vs Validation Accuracy
- Training vs Validation Loss

These plots help analyze:
- Learning stability
- Overfitting or underfitting
- Model convergence behavior

---

## 📈 Results
- **Training Accuracy:** ~99.4%
- **Validation Accuracy:** ~97.6%
- The ANN model successfully classifies handwritten digits
- Demonstrates strong generalization on unseen data
