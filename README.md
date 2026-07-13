# Parkinson's Disease Severity Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-green)
![Regression](https://img.shields.io/badge/Task-Regression-red)

## Overview

This project explores the use of Machine Learning regression models to predict the severity of Parkinson's disease from voice measurements. Using the **Oxford Parkinson's Disease Telemonitoring Dataset**, different preprocessing techniques, feature selection methods and regression algorithms were evaluated to identify the best-performing model.

## Dataset

- **Dataset:** Oxford Parkinson's Disease Telemonitoring Dataset (UCI Machine Learning Repository)
- **Samples:** 5,875 voice recordings
- **Patients:** 42 individuals diagnosed with Parkinson's disease
- **Features:** 22 variables, including 16 biomedical voice measurements
- **Target variables:** Clinical Parkinson's severity scores (UPDRS)

## Project Workflow

### 1. Data Preprocessing
- Loaded and explored the dataset
- Checked for missing and duplicate values
- Removed invalid observations (negative `test_time`)
- Performed exploratory data analysis (EDA)

### 2. Feature Selection
- Analysed feature correlations
- Removed highly correlated variables (correlation threshold > 0.95)
- Reduced redundancy while preserving relevant information

### 3. Model Development
The following regression algorithms were implemented and compared:

- Polynomial Regression
- Gradient Boosting Regressor
- Bayesian Ridge Regression

### 4. Model Optimisation
- Hyperparameter tuning using **GridSearchCV**
- Cross-validation using **GroupKFold** to ensure recordings from the same patient were not split across training and testing sets

### 5. Model Evaluation
Models were evaluated using:

- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Machine Learning Techniques

- Data preprocessing
- Exploratory Data Analysis (EDA)
- Feature selection
- Correlation analysis
- Regression modelling
- Hyperparameter optimisation
- Cross-validation
- Model evaluation

## Repository Structure

```
├── trab_AAEB_18_2_22_final.ipynb
├── README.md
└── data/
```

## Learning Outcomes

This project provided practical experience in:

- Building end-to-end Machine Learning pipelines
- Applying feature engineering and feature selection techniques
- Comparing multiple regression models
- Performing hyperparameter optimisation
- Evaluating predictive models using appropriate regression metrics
- Applying robust validation strategies with grouped cross-validation
