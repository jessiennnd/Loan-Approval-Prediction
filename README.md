# Loan Approval Prediction

## 📌 Project Overview  
This project analyzes a **Loan Approval dataset** (20,000 records) containing demographic, financial, and credit-related information.  
The main goal is to build and evaluate **classification models** that predict whether a loan application will be approved or denied.  

The project is divided into three major tasks:  
- **Data Cleaning & Preprocessing** – handling missing values, encoding categorical variables, and scaling features.  
- **Logistic Regression** – applying a supervised learning model to predict loan approval.  
- **K-Nearest Neighbors (K-NN)** – testing another supervised learning method to compare results.  

---

## 🔄 Workflow Summary  

### 🧹 Data Cleaning & Preprocessing  
- Removed irrelevant or redundant features.  
- Handled missing values and encoded categorical features.  
- Normalized numerical features for KNN.  

### 📊 Logistic Regression  
- Trained a logistic regression model using training data.  
- Evaluated with **accuracy, precision, recall, and F1-score**.  
- Used **RFE (Recursive Feature Elimination)** to identify the most important features.  

### 🤝 K-Nearest Neighbors (K-NN)  
- Experimented with different values of **k**.  
- Compared training vs. testing performance to check for **overfitting/underfitting**.  
- Chose the best **k** based on cross-validation and F1-score.  
