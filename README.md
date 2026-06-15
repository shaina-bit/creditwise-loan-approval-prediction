# CreditWise: Loan Approval Prediction using Machine Learning

Overview

CreditWise is a machine learning project that predicts whether a loan application is likely to be approved based on an applicant's financial and demographic information.

The project focuses on understanding the factors influencing loan approval decisions through Exploratory Data Analysis (EDA), feature engineering, and machine learning model comparison.

Problem Statement

Financial institutions must assess the creditworthiness of applicants before approving loans. Manual evaluation can be time-consuming and inconsistent.

This project aims to build a predictive system that can classify loan applications as:

Approved
Not Approved
using machine learning techniques.

Dataset Features

The dataset contains applicant information such as:

Gender
Marital Status
Education Level
Employer Category
Applicant Income
Savings
Credit Score
Debt-to-Income (DTI) Ratio
Loan Approval Status

Target Variable:

Loan_Approved

Exploratory Data Analysis (EDA)

Performed extensive data exploration and visualization, including:

Missing value analysis
Dataset statistics and distributions
Loan approval class balance analysis
Gender distribution analysis
Education level distribution
Marital status distribution
Employer category distribution
Correlation heatmap
Credit score vs loan approval analysis
Applicant income vs loan approval analysis
Outlier detection using box plots

Key Findings
Credit Score showed a strong relationship with loan approval.
Debt-to-Income Ratio influenced approval decisions.
Applicant income and savings contributed significantly to loan eligibility.
Certain demographic and employment characteristics impacted approval rates.

Data Preprocessing

The following preprocessing steps were performed:

Label Encoding of categorical features
Feature scaling using StandardScaler
Train-Test Split (80-20)

Feature Engineering

To capture non-linear relationships, additional features were created:

DTI_Ratio_sq
Credit_Score_sq

These engineered features helped improve model learning.

Machine Learning Models Used
Logistic Regression

A baseline linear classification model for predicting loan approval.

K-Nearest Neighbors (KNN)

A distance-based classification algorithm that classifies applicants based on neighboring samples.

Gaussian Naive Bayes

A probabilistic classification model based on Bayes' theorem.

Model Evaluation

Models were evaluated using:

Accuracy Score
Precision
Recall
F1 Score
Confusion Matrix

For loan approval prediction, special emphasis was placed on Precision and Recall, as misclassifying loan applications can have significant financial consequences.

Results

The performance of all three models was compared:

Logistic Regression
K-Nearest Neighbors (KNN)
Gaussian Naive Bayes
Best Performing Model

Logistic Regression Model (after feature engineering)
Precision:  0.7846153846153846
Accuracy:  0.88
Recall Score:  0.8360655737704918
F1 Score:  0.8095238095238095
Cpnfusion Matrix:  [[125  14]
 [ 10  51]]

KNN Model (after feature engineering)
Precision:  0.6730769230769231
Accuracy:  0.785
Recall Score:  0.5737704918032787
F1 Score:  0.6194690265486725
Cpnfusion Matrix:  [[122  17]
 [ 26  35]]

Naive Bayes Model (after feature engineering)
Precision:  0.8113207547169812
Accuracy:  0.86
Recall Score:  0.7049180327868853
F1 Score:  0.7543859649122807
Cpnfusion Matrix:  [[129  10]
 [ 18  43]]

Gaussian Naive Bayes achieved the strongest overall performance on the dataset and was selected as the best-performing model.

Technologies Used

Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-Learn
Jupyter Notebook

Project Workflow

Data Collection
Data Cleaning
Exploratory Data Analysis
Feature Engineering
Data Preprocessing
Model Training
Model Comparison
Performance Evaluation
Final Model Selection

Future Improvements

Hyperparameter tuning using GridSearchCV
Cross-validation for robust evaluation
Ensemble methods such as Random Forest and XGBoost
Model deployment using Streamlit
Real-time loan approval prediction dashboard

Author
Shaina Noushad
