# credit-risk-classification

## Overview of the Analysis

The purpose of this analysis was to evaluate a machine learning model's ability to predict loan statuses based on financial data. Specifically, the goal was to classify loans as either 0 (healthy loans) or 1 (high-risk loans).

The dataset included features such as income, debt, credit scores, and derogatory marks. The target variable, loan_status, indicated whether the loan was high-risk or not. The distribution of the target variable was skewed towards healthy loans, as indicated by the following breakdown:

Healthy loans (0): 96.8% of the data
High-risk loans (1): 3.2% of the data

The analysis involved the following stages:

Loading and exploring the dataset.
Splitting the data into training and testing sets.
Training a logistic regression model using the training data.
Evaluating the model’s performance using metrics such as accuracy, precision, recall, and f1-score.
The model used in this analysis was LogisticRegression, chosen for its simplicity and interpretability in binary classification tasks.

## Results

Machine Learning Model: Logistic Regression
Accuracy: 99%

Precision:
Healthy Loan (0): 1.00
High-Risk Loan (1): 0.84

Recall:
Healthy Loan (0): 0.99
High-Risk Loan (1): 0.94

F1-Score:
Healthy Loan (0): 1.00
High-Risk Loan (1): 0.89

## Summary

The logistic regression model performed exceptionally well overall, achieving a 99% accuracy rate. It demonstrated perfect precision and recall for healthy loans (0), making it highly reliable for identifying loans that are not high-risk. For high-risk loans (1), the model achieved strong recall (94%) but slightly lower precision (84%). This indicates that while the model identified most high-risk loans, some loans were incorrectly classified as high-risk.

## Recommendation

This model is well-suited for scenarios where it is more critical to minimize false negatives for high-risk loans, such as identifying loans that may require closer scrutiny. However, if further improvements are desired, the following steps could be considered:

Address class imbalance by oversampling the minority class (high-risk loans) or applying class weights in the logistic regression.

In conclusion, the logistic regression model is recommended due to its high overall performance and ease of implementation, making it a robust choice for predicting loan statuses.
