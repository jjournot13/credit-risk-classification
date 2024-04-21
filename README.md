# Module 12 Report

## Overview of the Analysis

The purpose of this project is to build a model that can identify the creditworthiness of borrowers. The dataset used includes historical lending activity from a peer-to-peer lending services company.

The dataset included 77,536 entries (75,036 healthy loans and 2,500 high-risk loans) with the following information:
- loan size
- interest rate
- borrower income
- debt to income ratio
- number of credit accounts
- number of deraogatory marks
- total debt
- current loan status

The target financial information used was loan status (label) and the remaining factors were used as features for the model.

The following steps were used for the machine learning process:
1. Created label and features sets.
1. Split the data into training and testing datasets by using train_test_split.
1. Created a Logistic Regression Model with the data.
1. Saved the predictions on the testing data labels and the fitted model.
1. Evaluated the model’s performance by generating a confusion matrix and classification report.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model - Logistic Regression

- Accuracy: 99%
- Precision: 100% for healthy loans/85% for high-risk loans
- Recall: 99% for healthy loans/91% for high-risk loans

## Summary

Based on the accuracy, precision and recall scores, the model appears to do well in predicting the health or risk of a loan, with healthy loans having more higher scores. However, it should be noted that the data is imbalanced with healthy loans having a significantly larger representation (75,036 entries versus 2,500), which likely skewed the results.

While this model should work for the company, I would like to either have a more balanced dataset to test in this model or use another model that can produce a more balanced comparison before making a recommendation.