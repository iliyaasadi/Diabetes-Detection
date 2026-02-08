📌 Overview

This project focuses on analyzing a large-scale clinical diabetes dataset to predict diabetes risk using machine learning and clustering techniques. It involves comprehensive exploratory data analysis, preprocessing, feature engineering, and the implementation of various classification and clustering models.

Developed as part of the Third Artificial Intelligence Project at Amirkabir University of Technology, this notebook provides an end-to-end pipeline for data science and predictive modeling in healthcare.

📊 Dataset

The dataset used is the "100,000 Diabetes Clinical Dataset" from Kaggle, containing anonymized patient records with the following features:

Features:

year: Year of record
gender: Gender of patient
age: Age of patient
location: Geographical location
race: One-hot encoded race categories
hypertension: Hypertension indicator
heart_disease: Heart disease indicator
smoking_history: Smoking status
bmi: Body Mass Index
hbA1c_level: HbA1c level
blood_glucose_level: Blood glucose level
diabetes: Target variable (0 = No Diabetes, 1 = Diabetes)

📈 Project Workflow

1. Data Loading & Exploration

Download dataset via Kaggle API
Perform initial inspection: missing values, data types, summary statistics
2. Exploratory Data Analysis (EDA)

Class imbalance analysis (pie charts, count plots)
Feature distribution and correlation analysis
Relationship between features and target variable
3. Data Preprocessing

Handling categorical variables (OneHotEncoder, LabelEncoder)
Scaling numerical features (StandardScaler)
Addressing class imbalance with SMOTE, SMOTEENN, and RandomUnderSampler
4. Clustering Analysis

Apply KMeans, Agglomerative Clustering, and DBSCAN
Evaluate clustering quality using silhouette score, Davies-Bouldin index, and Calinski-Harabasz score
5. Predictive Modeling

Train multiple classifiers:

Logistic Regression
Random Forest
XGBoost
Support Vector Machine (SVM)
Optimize hyperparameters using Optuna and GridSearchCV
Evaluate models with accuracy, F1-score, precision, recall, and confusion matrices
6. Model Interpretation & Validation

Cross-validation to ensure robustness
Visualize model performance and feature importance

🚀 How to Run

Clone or download the notebook.
Install required libraries:

bash
pip install opendatasets optuna xgboost imbalanced-learn plotly
Set up Kaggle API credentials (required for dataset download).
Run the notebook cells sequentially to reproduce the analysis and models.
