# Employee Attrition Prediction – IBM HR Analytics
Predicting which employees are at risk of leaving helps organizations take proactive measures to retain their talent. This project uses IBM’s fictional HR dataset to build and evaluate machine learning models for predicting employee attrition and understanding the key factors contributing to it.

## 📝 Table of Contents
Project Overview

Dataset

Project Goals

Project Structure

Methodology

Key Findings

Conclusion

## 📌 Project Overview
Employee attrition (voluntary resignations) is a critical problem for HR departments due to the costs associated with losing and replacing skilled workers. This project aims to:

Predict whether an employee is likely to leave the company.

Identify key features influencing employee attrition.

Evaluate model performance under different thresholds to optimize recall.

## 📂 Dataset
Source: IBM HR Analytics Employee Attrition & Performance (Fictional data).

Rows: 1470 employee records.

Features: 35+ attributes including demographic, job role, income, satisfaction metrics, etc.

Target: Attrition (Yes/No)

## 🎯 Project Goals

Perform Exploratory Data Analysis to understand the impact of various features on Attrition

Preprocess and explore the dataset.

Train multiple classification models:

Logistic Regression

Random Forest

XGBoost

Tune hyperparameters using RandomizedSearchCV with KFold cross-validation.

Evaluate models using precision, recall, F1-score, and accuracy.

Experiment with classification thresholds to improve recall (i.e., better detect likely leavers).

Analyze feature importance


## 📊 Methodology
Data Preprocessing:

Handled categorical encoding (OneHotEncoding).

Scaled numeric features using StandardScaler.

Model Training:

Split into training and testing sets

Trained models using RandomizedSearchCV + KFold cross-validation.

Tuned hyperparameters for each model.

Evaluation:

Metrics used: Accuracy, Precision, Recall, F1-score.

Tested multiple thresholds (e.g., 0.3, 0.4) to prioritize recall over accuracy.

Feature Importance:

Extracted Logistic Regression coefficients.

Identified top contributing features to attrition prediction.


🔍 Key Findings
Top features impacting attrition (from Logistic Regression coefficients):

OverTime

MaritalStatus_Single

JobInvolvement

StockOptionLevel

JobSatisfaction

EnvironmentSatisfaction

TotalWorkingYears

DistanceFromHome

MonthlyIncome

These insights can help HR teams prioritize retention strategies focused on high-risk profiles.

🧾 Conclusion
This project successfully built a machine learning pipeline to:

Predict employee attrition using classification models.

Tune models with cross-validation.

Improve recall by adjusting classification thresholds.

Interpret model coefficients to understand key attrition drivers.

These results provide valuable, actionable insights for HR departments aiming to improve employee retention.
