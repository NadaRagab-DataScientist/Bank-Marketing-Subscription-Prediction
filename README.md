# Bank Marketing Subscription Prediction

## Project Overview

This project predicts whether a customer will subscribe to a term deposit using machine learning models.

## Business Problem

Banks spend significant resources on marketing campaigns.
The objective is to identify customers who are most likely to subscribe to a term deposit and reduce unnecessary marketing costs.

## Dataset

- 11,162 records
- 16 Features
- Binary Classification

## Data Preprocessing

- Checked missing values
- Checked duplicates
- Feature Engineering
- Winsorization
- Label Encoding
- Standard Scaling (Logistic Regression)

## Models

- Logistic Regression
- Random Forest
- XGBoost

## Results

| Model | Accuracy | ROC-AUC |
|-------|---------|---------|
| Logistic Regression | 66.4% | 0.718 |
| Random Forest | 72.9% | 0.783 |
| XGBoost | 72.7% | 0.783 |

## Best Model

Random Forest achieved the best balance between Precision, Recall, F1-score and ROC-AUC.

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost



## Future Work

- Apply One-Hot Encoding for categorical variables.
- Experiment with CatBoost and LightGBM.
- Deploy the model using Streamlit.
- Optimize hyperparameters further.
