# Loan Approval Prediction (Supervised machine learning project)

This is my project to practice machine learning, mainly logistic regression and KNN, and to get hands-on with feature selection, model evaluation, and predictive analytics.

## Project Overview
This project analyzes a **Loan Approval dataset** (20,000 records) containing demographic, financial, and credit-related information.  
The main goal is to build and evaluate classification models that predict whether a loan application will be approved or denied.  

The tasks completed include:  
- Data Cleaning & Preprocessing – preparing the dataset for analysis.  
- Logistic Regression – applying a linear classification model to predict loan approval.  
- K-Nearest Neighbors (KNN) – testing another supervised learning method to compare results.  

---

## Dataset Information
The dataset is a modified version of the *Synthetic Dataset for Risk Assessment and Loan Approval Modeling* shared by Lorenzo Zoppelletto.  
It comprises 20,000 records of personal and financial data, providing a comprehensive basis for predictive modeling.  


## Workflow

### Data Cleaning & Preprocessing
- Removed irrelevant or redundant features.  
- Handled missing values and encoded categorical variables.  
- Scaled numerical features for KNN.  

### Logistic Regression
- Trained a logistic regression model using training data (Used 80% of data for training and 20% for testing).  
- Used Recursive Feature Elimination (RFE) to identify the most important features.  

### K-Nearest Neighbors (KNN)
- Performed Recursive Feature Elimination (RFE) for feature selection.  
- Started with 1-NN classifier and evaluated training vs. testing performance.  
- Identified potentialoverfitting issues in small-k values.  
- Conducted Grid Search with cross-validation to find the optimal `k`.  
- Visualized accuracy trends across different values of `k`.  
- Compared distance metrics: Euclidean, L1 (Manhattan), and Cosine.  
- Selected the best configuration based on F1-score and cross-validation accuracy.

## Key Insight
Logistic Regression performed slightly better overall as its predictions on testing data were more accurate and balanced. KNN was close but a tiny bit lower, especially in F1-score. It may be due to Logistic Regression can capture the overall patterns more efficiently with selected features, while KNN depends on local similarities and can be affected by data density or noise.
