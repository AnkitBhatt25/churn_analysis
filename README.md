

#  Customer Churn Analysis & Dashboard

This repository contains two projects focused on Customer Churn Analysis using both **Machine Learning** and **Business Intelligence (Power BI)**. The dataset used is the **Telco Customer Churn Dataset**, which includes customer demographics, subscription details, and churn labels.

---

## 1️ Churn Analysis (Machine Learning)

###  Overview
The churn analysis project focuses on predicting customer churn using a **machine learning pipeline**. The dataset consists of both categorical and numerical customer attributes.

###  Steps Performed
- **Data Cleaning & Preprocessing**
  - Handled missing values and categorical encoding.
  - Balanced the dataset using **SMOTE (Synthetic Minority Oversampling Technique)** since churn distribution was skewed.

- **Exploratory Data Analysis (EDA)**
  - Performed **univariate & bivariate analysis** to identify churn drivers.
  - Built correlation heatmaps for feature importance.

- **Model Training & Evaluation**
  - Models tested: `Logistic Regression`, `Random Forest`, `Gradient Boosting (XGBoost/LightGBM)`.
  - ✅ Final selected model: **Gradient Boosting**, due to the best validation performance.

###  Results
- **Accuracy**: ~82%  
- **F1-Score (Churn class)**: 0.79  
- **Key Drivers Identified**: Contract type, tenure, monthly charges, internet service type  

###  Tools & Libraries
- Python, Pandas, NumPy, Matplotlib, Seaborn  
- Scikit-learn (model building & evaluation)  
- Imbalanced-learn (SMOTE for balancing classes)  

---

## 2️ Churn Dashboard (Power BI)

###  Overview
The **Power BI dashboard** is built on the same Telco Customer Churn dataset but focuses on **historical churn analysis** (no ML integration). It provides an **interactive and visual summary** of churn trends for business decision-making.

###  Features
- **KPIs**
  - Total Customers  
  - Churn Rate (%)  
  - Average Tenure  

- **Visuals**
  - Churn breakdown by gender, contract type, and payment method   
  - Donut charts for churn vs. non-churn distribution  


### 🛠️ Tools
- Power BI Desktop  
- DAX (for measures & calculations)  

---

