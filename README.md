# Credit-Risk-Classification_challenge
Assignment 20

## Overview of the Analysis
Purpose of the Analysis: The primary purpose of this analysis was to build and evaluate a machine learning model that can predict the creditworthiness of borrowers. Using historical lending data from a peer-to-peer lending services company, the goal was to identify loans that are at high risk of defaulting (label 1) and those that are healthy (label 0).

### Financial Information and Prediction: 
The dataset contains financial information about borrowers, including loan amounts, interest rates, borrower incomes, and other relevant factors. The target variable to predict is the loan_status, where 0 indicates a healthy loan and 1 indicates a high-risk loan.

### Variables Overview:
* The target variable (loan_status) has two values: 0 (healthy loan) and 1 (high-risk loan).

### Stages of the Machine Learning Process:
1. Data Loading: Read the data from lending_data.csv into a Pandas DataFrame.
2. Data Preparation: Separate the data into labels (y) and features (X).
3. Data Splitting: Split the data into training and testing sets using train_test_split.
4. Model Training: Train a logistic regression model using the training data.
5. Model Prediction: Use the trained model to make predictions on the testing data.
6. Model Evaluation: Evaluate the model's performance using a confusion matrix and classification report.

### Methods Used:
* Logistic Regression: This method was used to build the predictive model. Logistic regression is a statistical method for predicting binary outcomes.

### Results: 
Machine Learning Model 1: Logistic Regression
* Accuracy Score: 99%
* Precision and Recall Scores:
  - For 0 (healthy loan):
    - Precision: 1.00
    - Recall: 0.99
    - F1-Score: 1.00
* For 1 (high-risk loan):
    - Precision: 0.85
    - Recall: 0.94
    - F1-Score: 0.89

### Summary:  
Model Performance: The logistic regression model demonstrates excellent performance overall, with an accuracy score of 99%. The model predicts healthy loans with near-perfect precision (1.00) and recall (0.99). It also performs well in predicting high-risk loans, with a precision of 0.85 and a recall of 0.94.

### Recommendation:  
Based on the evaluation metrics, the logistic regression model is recommended for use by the company. The high precision and recall values for both healthy and high-risk loans indicate that the model is reliable and can effectively identify creditworthy borrowers while minimizing the risk of misclassifying high-risk loans.

### Considerations:  
The performance of the model depends on the problem we are trying to solve. In this case, it is crucial to balance the prediction of both 0 and 1 labels to ensure that healthy loans are correctly identified and high-risk loans are not overlooked.
If predicting high-risk loans (1) is more critical for the business, the model's recall for this label (0.94) suggests it performs well in identifying most high-risk loans.