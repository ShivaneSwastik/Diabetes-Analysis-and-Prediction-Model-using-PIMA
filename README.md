# Diabetes-Analysis-and-Prediction-Model-using-PIMA
**Early Diabetes Risk Prediction & Clinical Feature Engineering Pipeline**
**Overview**:- This repository contains an end-to-end Machine Learning and Exploratory Data Analysis (EDA) pipeline for early diabetes prediction using the PIMA Indians Diabetes Dataset. Rather than relying solely on default metrics, this project highlights clinical domain feature engineering, data quality remediation, and comparative statistical modeling to evaluate female patients' diabetes risks accurately.
**Key Features & Methodology**:-
**Clinical Data Remediation**: Identified and isolated biologically impossible values (e.g., zero entries for BMI, Blood Pressure, and Insulin) to prevent data distortion, transitioning between full-dataset distributions and complete-case analysis ($n=392$).
**Domain-Specific Feature Engineering**: Constructed clinically actionable features based on established medical guidelines:
       OGTT Glucose Categorization: Segmented glucose tolerance levels (Normal, Impaired, Diagnostic).
       Nutritional Status: Grouped continuous BMI values into WHO-aligned categories (Underweight, Normal, Overweight, Obese).
       Age-Adjusted Skinfold Percentiles: Engineered multi-tier percentile features for triceps skinfold thickness.
**Multi-Model Machine Learning:** Implemented, benchmarked, and cross-validated several classification algorithms:Logistic Regression (with statistical p-value evaluation via statsmodels)
           Support Vector Machines (SVM)
           K-Nearest Neighbors (KNN)
           Naive Bayes (MultinomialNB)
**Feature Selection & Optimization**: Utilized Recursive Feature Elimination with Cross-Validation (RFECV) alongside K-Fold and Stratified K-Fold strategies to select optimal clinical predictors and prevent overfitting.
**Diagnostic Performance Evaluation**: Prioritized Sensitivity (Recall), Precision-Recall Curves, and ROC-AUC metrics to minimize false negatives in diagnostic classification.

**Tech Stack**
Language: Python 3.12
Data Processing & EDA: Pandas, NumPyData Visualization: Seaborn, Matplotlib
Machine Learning & Statistics: Scikit-Learn, Statsmodels , PyCaret.
