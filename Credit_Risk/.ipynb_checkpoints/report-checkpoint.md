# Module 20 Report

## Overview of the Analysis

The analysis involved developing machine learning models to assess credit risk. Specifically, we aimed to predict the likelihood of a loan being a "healthy loan" (0) or a "high-risk loan" (1) based on financial information. The data included features like loan size, interest rate, borrower income, and debt-to-income ratio. The `value_counts` of the target variable indicated an imbalanced classification problem, with significantly more healthy loans than high-risk loans.

The machine learning process included:
- Data preprocessing (splitting, encoding, scaling)
- Splitting data into training and testing sets
- Balancing the data using `RandomOverSampler`
- Fitting models using `LogisticRegression`

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

The Logistic Regression model with resampled training data (Model 2) outperformed the original model, particularly in balancing the prediction accuracy for both classes, as evidenced by the higher balanced accuracy score. While both models show high precision and recall, the resampled model has a significant edge in identifying high-risk loans, which is crucial for credit risk assessment.

**Recommendation**: Model 2, the Logistic Regression with resampled training data, should be used for credit risk prediction. This model's ability to better identify high-risk loans can be particularly valuable for financial institutions looking to minimize risk.
