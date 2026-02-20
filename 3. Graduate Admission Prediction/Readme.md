# 🎓 Graduate Admission Prediction using Artificial Neural Networks (ANN)

## 🔍 Project Overview
This project predicts the **probability of admission to a graduate program** based on a student’s academic profile using an **Artificial Neural Network (ANN)**.

The model learns relationships between standardized test scores, academic performance, and research experience to estimate the **Chance of Admit**.  
The project demonstrates a complete machine learning workflow including data preprocessing, feature scaling, ANN model training, evaluation, and performance visualization.

---

## 🧠 Problem Statement
Given a set of applicant attributes, predict the **Chance of Admission** to a graduate program.

This is a **regression problem**, where the output is a continuous probability score between `0` and `1`.

---

## 🗂️ Dataset Information
- **Dataset File:** Graduate Admission Dataset (CSV)
- **Problem Type:** Regression

### Features Used
- GRE Score  
- TOEFL Score  
- University Rating  
- Statement of Purpose (SOP)  
- Letter of Recommendation (LOR)  
- CGPA  
- Research Experience  

### Target Variable
- **Chance of Admit**

---

## 🛠️ Technologies & Tools
- **Programming Language:** Python  
- **Libraries:** NumPy, Pandas, Matplotlib  
- **Machine Learning:** Scikit-learn  
- **Deep Learning:** TensorFlow, Keras  

---

## 🔄 Project Workflow

### 1️⃣ Data Loading & Exploration
- Loaded the dataset using Pandas
- Inspected feature distributions and dataset structure
- Verified data types and numerical consistency

---

### 2️⃣ Data Preprocessing
- Separated features (`X`) and target (`y`)
- Dataset contains only numerical values, so no categorical encoding was required

---

### 3️⃣ Train-Test Split
- Split the dataset into **80% training** and **20% testing**
- Ensured unbiased evaluation on unseen data

---

### 4️⃣ Feature Scaling
- Applied **StandardScaler** to normalize input features
- Improved ANN training stability and convergence

---

### 5️⃣ Model Building (ANN)
- Built a Sequential Artificial Neural Network
- Architecture includes:
  - Dense hidden layers with **ReLU activation**
  - Output layer with **Linear activation**
- Designed specifically for regression tasks

---

### 6️⃣ Model Compilation
- **Loss Function:** Mean Squared Error (MSE)  
- **Optimizer:** Adam  

---

### 7️⃣ Model Training
- Trained the model for **100 epochs**
- Training loss monitored to ensure proper convergence

---

### 8️⃣ Model Evaluation
- Generated predictions on test data
- Evaluated model performance using **R² Score**

**R² Score:**  `0.8279446184141058`


The R² score indicates that the model explains approximately **82.8% of the variance** in admission probability.

---

### 9️⃣ Performance Visualization
- Training Loss vs Epochs plot
- Used to analyze:
  - Learning stability
  - Model convergence
  - Overfitting or underfitting behavior

---

## 📈 Results
- The ANN model successfully captures patterns in graduate admission data
- Achieves a strong **R² score of 0.828**
- Demonstrates good generalization on unseen applicant profiles
