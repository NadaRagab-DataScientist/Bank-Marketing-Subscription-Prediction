# Bank Marketing Subscription Prediction

Machine Learning project for predicting whether a customer will subscribe to a bank term deposit using Logistic Regression, Random Forest, and XGBoost.

---

## Project Overview

This project aims to predict whether a bank customer will subscribe to a term deposit based on demographic information and previous marketing campaign interactions.

The project covers the complete machine learning workflow, including data exploration, preprocessing, feature engineering, model training, evaluation, and hyperparameter tuning.

---

## Business Problem

Banks invest significant resources in marketing campaigns. Contacting every customer is costly and inefficient.

The goal of this project is to identify customers who are more likely to subscribe to a term deposit, helping banks improve campaign efficiency and reduce marketing costs.

---

## Dataset

- **11,162** customer records
- **16** input features
- Binary Classification
- Target Variable: **deposit (Yes / No)**

---

## Data Preprocessing

- Checked missing values
- Checked duplicate records
- Investigated "unknown" categorical values
- Feature Engineering (`never_contacted`)
- Winsorization for outlier handling
- Label Encoding for categorical variables
- Standard Scaling (Logistic Regression only)
- Train/Test Split with Stratification

---

## Machine Learning Models

- Logistic Regression (Baseline)
- Random Forest
- XGBoost

---

## Model Performance

| Model | Accuracy | ROC-AUC |
|--------|---------:|---------:|
| Logistic Regression | 66.4% | 0.718 |
| Random Forest | **72.9%** | **0.783** |
| XGBoost | 72.7% | 0.783 |

---

## Best Model

Random Forest was selected as the final model because it achieved the highest overall performance and the best balance between Accuracy, Precision, Recall, F1-score, and ROC-AUC.

Additionally:

- Cross Validation was performed to evaluate model generalization.
- Hyperparameter Tuning was applied using GridSearchCV.
- Feature Importance analysis was used to interpret the model.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- SciPy

---

## Project Structure

```text
Bank-Marketing-Subscription-Prediction
│
├── data/
│   └── bank.csv
│
├── images/
│
├── Bank.ipynb
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

## Visualizations

### Model Comparison

![Model Comparison](images/model_comparison.png)

### Feature Importance

![Feature Importance](images/feature_importance.png)

### ROC Curve

![ROC Curve](images/roc_curve.png)

### Confusion Matrix

![Confusion Matrix](images/confusion_matrix.png)

---

## Future Work

- Apply One-Hot Encoding instead of Label Encoding.
- Experiment with CatBoost and LightGBM.
- Perform additional feature selection techniques.
- Deploy the model using Streamlit or Flask.
- Explore advanced hyperparameter optimization methods.

---

## Conclusion

Three machine learning models were evaluated to predict customer subscription to a bank term deposit.

Random Forest achieved the best overall performance and was selected as the final model. The project demonstrates a complete end-to-end machine learning pipeline, from data preprocessing and feature engineering to model evaluation, interpretation, and optimization.
