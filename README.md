# Creditworthiness Classifier - Analysis of Logistic Regression Models

<br>

## Overview of the Analysis

The purpose of this analysis is to determine if the assessment of the creditworthiness of borrowers on peer-to-peer lending platforms can be automated using a classification model. The model was trained with historical data comprising a target of loan default status (75,036 compliant, 2,500 non-compliant) and the following features:  

  * Loan Size
  * Interest Rate
  * Borrower Income
  * Debt-to-Income Ratio
  * Number of Accounts
  * Derogatory Marks
  * Total Debt

The analysis followed the standard convention of model-fit-predict-evaluate. Logistic Regression is used as the baseline. The model is trained with the raw data and balanced data using random oversampling to address the imbalance in the target variable.

## Results

The models are evaluated using accuracy, precision, and recall. The precision and recall values represent the label of interest, that is, non-compliant loans.

* Logistic Regression - Imbalanced Training Set:
  * Accuracy: 0.94
  * Precision: 0.84
  * Recall: 0.89



* Logistic Regression - Balanced Training Set:
  * Accuracy: 0.99
  * Precision: 0.84
  * Recall: 0.99

## Summary

Both Logistic Regression models performed quite well. Training the Logistic Regression model with the randomly oversampled dataset increased both accuracy and recall without any sacrifice in precision. Future work to develop a better model should use the Logistic Regression model trained with the balanced dataset as the baseline. The same model is also recommended if deploying a model in an alpha-testing phase at this moment.
