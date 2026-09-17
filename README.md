# Diabetes Risk Prediction and Health Analysis

A machine learning project that explores diabetes-related health indicators and compares multiple classification models to predict whether an individual is diagnosed with diabetes.

## Project Overview

Early identification of diabetes risk can support preventive healthcare and encourage timely medical screening. This project analyzes a dataset containing 100,000 records with demographic information, lifestyle habits, family history, and clinical health indicators.

The project focuses on:

- Exploring patterns associated with diabetes diagnosis
- Identifying important health and lifestyle-related features
- Comparing different classification algorithms
- Handling class imbalance with SMOTE
- Improving model performance through hyperparameter tuning

## Dataset

The dataset contains 100,000 records and 31 features, including:

- Demographic information: age, gender, ethnicity, education level, and income level
- Lifestyle factors: smoking status, alcohol consumption, physical activity, diet, sleep, and screen time
- Medical history: family history of diabetes, hypertension, and cardiovascular disease
- Clinical indicators: BMI, blood pressure, cholesterol, glucose, insulin, HbA1c, and heart rate
- Target variable: `diagnosed_diabetes`

## Analytical Workflow

1. Data inspection and exploratory data analysis
2. Duplicate and missing-value checks
3. Univariate and multivariate analysis
4. Correlation analysis
5. Feature preprocessing:
   - Standardization for numerical variables
   - Ordinal encoding for ordered categorical variables
   - One-hot encoding for nominal categorical variables
6. Train-test split using a 70/30 ratio
7. Model training and evaluation
8. Class imbalance handling with SMOTE
9. Feature selection
10. XGBoost hyperparameter tuning

## Models Evaluated

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

The models were evaluated using:

- Accuracy
- F1-score
- ROC-AUC
- Confusion matrix
- False positives and false negatives

## Key Results

Random Forest and XGBoost achieved the strongest overall performance among the evaluated models, with approximately:

- Accuracy: 0.92
- F1-score: 0.91
- ROC-AUC: 0.93

The analysis also showed that reducing false negatives remains an important challenge, since incorrectly classifying a person with diabetes as negative may have serious consequences.

## Selected Features

The feature-selection experiment focused on:

- `diabetes_risk_score`
- `hba1c`
- `glucose_fasting`
- `glucose_postprandial`
- `family_history_diabetes`

## Recommendations

Based on the analysis, the project recommends:

- Collecting more relevant and reliable health data
- Increasing public screening and education around diabetes risk factors
- Including additional health indicators to improve prediction of diabetes type and stage
- Developing a user-friendly diabetes risk assessment tool

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- XGBoost
- Google Colab
- Jupyter Notebook

## Project Files

- `DA90_FinalProject.ipynb`: Complete analysis and machine learning workflow
- `DA90_Tam+Lam_FinalProject.pdf`: Project presentation and results

## Contributors

- Le Huynh Minh Tam
- Vu Tran Vy Lam

## Disclaimer

This project is for educational and analytical purposes only. The model is not intended to provide medical diagnosis or replace professional medical advice.
