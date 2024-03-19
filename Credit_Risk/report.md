# Module 20 Report

## Overview of the Analysis

The analysis encompassed the development of machine learning models to evaluate credit risk, focusing on predicting whether a loan is classified as a "healthy loan" (0) or a "high-risk loan" (1) based on financial attributes. Data features comprised metrics such as loan size, interest rate, borrower income, and debt-to-income ratio. Notably, the value_counts of the target variable highlighted an imbalanced classification issue, with a notably higher count of healthy loans compared to high-risk ones.

The machine learning workflow entailed several key steps:

Data preprocessing, including splitting, encoding, and scaling
Segregation of data into training and testing sets
Balancing the dataset using the RandomOverSampler technique
Model fitting using the LogisticRegression algorithm


## Results

The performance of two machine learning models was assessed:

* **Machine Learning Model 1**: Original Logistic Regression
  * Balanced Accuracy Score: 95.204%
  * Precision: Healthy Loan (0) - 100%, High-Risk Loan (1) - 86%
  * Recall: Healthy Loan (0) - 100%, High-Risk Loan (1) - 90%
  
* **Machine Learning Model 2**: Logistic Regression with Resampled Training Data
  * Balanced Accuracy Score: 99.368%
  * Precision: Healthy Loan (0) - 100%, High-Risk Loan (1) - 84%
  * Recall: Healthy Loan (0) - 99%, High-Risk Loan (1) - 99%

## Summary

The Logistic Regression model trained on resampled data (Model 2) demonstrated superior performance compared to the original model, notably in achieving a more balanced prediction accuracy across both classes, as indicated by the increased balanced accuracy score. Although both models exhibited high precision and recall, the resampled model notably excelled in identifying high-risk loans, a critical aspect in credit risk assessment.

**Recommendation**: Model 2, the Logistic Regression trained on resampled data, is recommended for credit risk prediction. Its enhanced capability to accurately identify high-risk loans can be especially advantageous for financial institutions aiming to mitigate risks effectively.