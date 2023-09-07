# Credit Risk Classification Report

## Overview of the Analysis

### Purpose of the Analysis
The primary aim of this analysis is to assess the creditworthiness of borrowers using historical lending data. By leveraging machine learning, we aim to create a model that can accurately identify the risk associated with each loan—either "healthy" (`0`) or "high-risk" (`1`).

### Financial Information
The dataset comprises various financial metrics and attributes of borrowers, with the target variable being the "loan_status" which we needed to predict.

### Variables
- The `loan_status` column contains the labels:
  - 0: Healthy loan
  - 1: High-risk loan

### Stages and Methods
The machine learning process involved the following stages:
1. Data Preparation: Reading the data, splitting into features (X) and labels (y).
2. Data Splitting: Dividing the dataset into training and testing sets.
3. Model Training: Using Logistic Regression to fit the training data.
4. Model Evaluation: Analyzing performance using metrics like accuracy, precision, and recall.

## Results

### Logistic Regression Model with Original Data
- **Accuracy**: 99%
- **Precision**: 
  - High-risk: 1.00
  - Low-risk: 0.85
- **Recall**: 
  - High-risk: 0.99
  - Low-risk: 0.91

### Logistic Regression Model with Oversampled Data
- **Accuracy**: 99%
- **Precision**: 
  - High-risk: 1.00
  - Low-risk: 0.84
- **Recall**: 
  - High-risk: 0.99
  - Low-risk: 0.99

## Summary

### Best Performing Model
The Logistic Regression Model with oversampled data appears to perform slightly better overall, particularly when it comes to identifying high-risk loans. The recall for high-risk loans is at 99%, meaning it captures almost all of the high-risk cases.

### Problem-Specific Performance
Given the nature of credit risk, it's crucial to correctly identify high-risk loans (`1`s) to mitigate potential financial loss. Therefore, the higher recall score for high-risk loans in the oversampled model makes it more suitable for this specific problem.

### Recommendation
I recommend the Logistic Regression Model with oversampled data for predicting the credit risk due to its high accuracy and exceptional recall rate for high-risk loans. This model is reliable for both identifying healthy loans and flagging those that are high-risk, thereby offering a balanced and efficient solution for credit risk assessment.