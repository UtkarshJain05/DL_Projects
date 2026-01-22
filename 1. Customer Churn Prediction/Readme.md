# 📊 Customer Churn Prediction using Artificial Neural Networks (ANN)

## 🔍 Project Overview
Customer churn has a direct impact on business revenue. This project builds an end-to-end **Customer Churn Prediction system** using an **Artificial Neural Network (ANN)** to predict whether a customer is likely to leave a bank based on historical customer data.

The project demonstrates the complete machine learning workflow, including data preprocessing, feature engineering, neural network modeling, evaluation, and performance visualization.

---

## 🧠 Problem Statement
Predict whether a customer will **churn (exit)** based on demographic and financial attributes so that businesses can take proactive retention actions.

**Target Variable:**
- `Exited = 1` → Customer churned  
- `Exited = 0` → Customer retained  

---

## 🗂️ Dataset Information
- **Dataset File:** `Churn_Modelling.csv`
- **Problem Type:** Binary Classification

### Features Used
- Credit Score  
- Geography  
- Gender  
- Age  
- Tenure  
- Balance  
- Number of Products  
- Has Credit Card  
- Is Active Member  
- Estimated Salary  

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
- Checked data types, missing values, and duplicates
- Analyzed target variable distribution

---

### 2️⃣ Data Preprocessing
- Removed irrelevant columns:
  - `RowNumber`
  - `CustomerId`
  - `Surname`
- Applied One-Hot Encoding on categorical variables:
  - `Geography`
  - `Gender`
- Avoided dummy variable trap using `drop_first=True`

---

### 3️⃣ Train-Test Split
- Separated features (`X`) and target (`y`)
- Split data into **80% training** and **20% testing**

---

### 4️⃣ Feature Scaling
- Used **StandardScaler** to normalize feature values
- Improved ANN convergence and performance

---

### 5️⃣ Model Building (ANN)
- Built a Sequential Neural Network
- Hidden layers with **ReLU activation**
- Output layer with **Sigmoid activation**
- Designed for binary classification

---

### 6️⃣ Model Compilation
- **Loss Function:** Binary Crossentropy  
- **Optimizer:** Adam  
- **Metric:** Accuracy  

---

### 7️⃣ Model Training
- Trained the model for **100 epochs**
- Used **20% validation split**
- Stored training history for visualization

---

### 8️⃣ Model Evaluation
- Generated predictions on test data
- Converted probabilities to binary outputs using threshold `0.5`
- Evaluated performance using:
  - Accuracy Score
  - Confusion Matrix

---

### 9️⃣ Performance Visualization
- Training vs Validation Accuracy
- Training vs Validation Loss

These visualizations help understand model learning behavior and generalization.

---

## 📈 Results
- The ANN model successfully learns customer churn patterns
- Validation trends indicate stable learning
- Model performs well on unseen test data
