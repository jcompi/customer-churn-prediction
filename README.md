# Customer Churn Prediction

## Overview
This project aims to predict customer churn using machine learning techniques.  
Customer churn prediction is a critical task for businesses, as identifying customers likely to leave allows companies to take proactive retention measures.

## Dataset
IBM Telco Customer Churn Dataset  
The dataset contains customer demographic information, service usage details, and billing data.

## Objectives
- Perform exploratory data analysis (EDA)
- Clean and preprocess the dataset
- Build a predictive model to classify churn
- Evaluate model performance with business-oriented metrics

## Data Preprocessing
- Converted categorical variables using one-hot encoding
- Handled missing values in `TotalCharges`
- Scaled numerical features for model training
- Split dataset into training and testing sets (80/20)

## Modeling
Two Logistic Regression models were trained:

1. Baseline Model  
   - Accuracy: ~78%  
   - Recall (Churn): ~52%

2. Balanced Model (class_weight='balanced')  
   - Accuracy: ~73%  
   - Recall (Churn): ~79%

## Key Insight
Although the balanced model slightly reduced overall accuracy, it significantly improved churn detection.  
In business contexts, maximizing recall for churn is often more valuable than maximizing overall accuracy.

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## Conclusion
The project demonstrates an end-to-end data science workflow:
data cleaning, exploratory analysis, model building, evaluation, and business interpretation.

Future improvements could include:
- Trying tree-based models (Random Forest, XGBoost)
- Hyperparameter tuning
- Cross-validation
- Feature importance analysis
