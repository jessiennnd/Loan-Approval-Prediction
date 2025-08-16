# Loan Approval Prediction

## 📌 Project Overview
This project analyzes a **Loan Approval dataset** (20,000 records) containing demographic, financial, and credit-related information.  
The main goal is to build and evaluate **classification models** that predict whether a loan application will be **approved or denied**.  

The tasks completed include:  
- **Data Cleaning & Preprocessing** – preparing the dataset for analysis.  
- **Logistic Regression** – applying a linear classification model to predict loan approval.  
- **K-Nearest Neighbors (KNN)** – testing another supervised learning method to compare results.  

---

## 📂 Dataset Information
The dataset is a modified version of the *Synthetic Dataset for Risk Assessment and Loan Approval Modeling* shared by **Lorenzo Zoppelletto**.  
It comprises **20,000 records** of personal and financial data, providing a comprehensive basis for predictive modeling.  

### 🔑 Key Features
Some of the main columns include:  

| Column | Meaning |
|--------|---------|
| ApplicationDate | Loan application date |
| Age | Applicant's age |
| AnnualIncome | Yearly income |
| CreditScore | Creditworthiness score |
| EmploymentStatus | Job situation |
| EducationLevel | Highest education attained |
| LoanAmount | Requested loan size |
| LoanDuration | Loan repayment period |
| MaritalStatus | Applicant's marital state |
| DebtToIncomeRatio | Debt to income proportion |
| PaymentHistory | Past payment behavior |
| TotalAssets | Total owned assets |
| TotalLiabilities | Total owed debts |
| LoanApproved | **Target variable: loan approval status** |
| RiskScore | Risk assessment score |

---

## Workflow

### Data Cleaning & Preprocessing
- Removed irrelevant or redundant features.  
- Handled missing values and encoded categorical variables.  
- Scaled numerical features for KNN.  

### Logistic Regression
- Trained a logistic regression model using training data.  
- Evaluated with **accuracy, precision, recall, and F1-score**.  
- Used **Recursive Feature Elimination (RFE)** to identify the most important features.  

### K-Nearest Neighbors (KNN)
- Performed **Recursive Feature Elimination (RFE)** for feature selection.  
- Started with **1-NN classifier** and evaluated training vs. testing performance.  
- Identified potential **overfitting** issues in small-k values.  
- Conducted **Grid Search with cross-validation** to find the optimal `k`.  
- Visualized accuracy trends across different values of `k`.  
- Compared distance metrics: **Euclidean, L1 (Manhattan), and Cosine**.  
- Selected the best configuration based on **F1-score and cross-validation accuracy**.  
