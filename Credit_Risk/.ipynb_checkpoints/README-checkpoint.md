# Credit Risk Prediction

## Overview

This project focuses on predicting credit risk using machine learning models. The goal is to distinguish between "healthy loans" and "high-risk loans" based on financial data, using a logistic regression model. The dataset includes various financial metrics such as loan size, interest rate, borrower income, and debt-to-income ratio.

## Table of Contents

- [Installation](#installation)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Results](#results)

## Installation

To run this project, you will need to install Python and the necessary libraries:

```bash
pip install pandas scikit-learn imbalanced-learn 
```

## Modeling

Two logistic regression models were developed:

1. A baseline logistic regression model with the original dataset.
2. A logistic regression model with oversampled training data using `RandomOverSampler`.

## Evaluation

The models were evaluated based on:

- Balanced accuracy score
- Precision and recall scores
- Confusion matrix
- Classification report

## Results

The results showed that:

- The oversampled logistic regression model had a higher balanced accuracy score, suggesting better performance in predicting both classes.
- Both models showed high precision and recall for healthy loans, with the oversampled model also demonstrating high recall for high-risk loans.

