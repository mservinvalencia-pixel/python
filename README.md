# Python Churn Project
# Bank Customer Churn Analysis

## Overview

This project focuses on analyzing and predicting customer churn using a banking dataset. The objective is to identify the main factors associated with customer attrition and build machine learning models capable of estimating the probability that a customer will leave the service.

The workflow combines exploratory data analysis (EDA), data preprocessing, handling class imbalance, and predictive modeling.

---

## Dataset

The dataset used in this project contains **10,000 observations and 14 variables**, including customer demographics, financial information, and account activity.

Typical features include:

* Credit score
* Geography
* Gender
* Age
* Tenure
* Balance
* Number of products
* Has credit card
* Is active member
* Estimated salary
* Churn (target variable)

---

## Project Workflow

### 1. Data Loading and Exploration

* Load dataset from a CSV file
* Inspect structure, data types, and missing values
* Perform descriptive statistics

### 2. Exploratory Data Analysis (EDA)

* Analyze churn distribution
* Explore relationships between features and churn
* Visualize patterns (age, balance, geography, etc.)

### 3. Data Preprocessing

* Remove non-informative features (e.g., IDs)
* Encode categorical variables (One-Hot Encoding)
* Scale numerical features (Standardization)

### 4. Train-Test Split

* Split dataset into training and testing sets

### 5. Handling Class Imbalance

* Detect imbalance in churn vs non-churn
* Apply **SMOTE (Synthetic Minority Oversampling Technique)**

### 6. Model Training

Train and compare multiple models:

* Logistic Regression
* Random Forest
* XGBoost

### 7. Model Evaluation

Evaluate models using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* Classification Report

### 8. Hyperparameter Tuning

* Use **GridSearchCV** with cross-validation
* Optimize model performance

---

## Key Findings

* Churn is strongly associated with variables such as:

  * Age
  * Account balance
  * Geography
* The dataset is **highly imbalanced**, making accuracy alone an unreliable metric
* SMOTE improves recall for the minority class (churn), at the cost of slight accuracy trade-offs

---

## Results

* Random Forest achieved strong baseline performance (~0.87 accuracy)
* Tuned models and SMOTE versions improved detection of churned customers
* Trade-off observed between overall accuracy and recall for the minority class

---

## Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Imbalanced-learn (SMOTE)
* Matplotlib
* Seaborn

---

## Conclusion

This project demonstrates how to:

* Perform end-to-end churn analysis
* Handle class imbalance effectively
* Compare multiple machine learning models
* Build a robust pipeline for customer attrition prediction

---

## Future Improvements

* Feature engineering (behavioral features, ratios, etc.)
* Model explainability (SHAP, feature importance)
* Deployment as an API or dashboard
* Real-time churn prediction

---

## Author

Data Science project focused on churn prediction and applied machine learning.

