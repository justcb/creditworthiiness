LogisticRegression Model Applied to Creditworthiness

## Overview of the Analysis

This report is based on analysis using various techniques to train and evaluate machine learing models. This report pulls from a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

The historical lending activity data contains the following data about borrowers: loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, and total_debt.  In addtion, the table contains an evaluation of the current status of the borrower's loan.

Ultimately, the goal of the model is to be able to accurately identify high-risk borrowers.  To accomplish this, a LogisticRegression model was created, fit, and its predictions evaluated.  Subsequently, the data was randomly oversampled to create more balance between the number of datapoints for healthy v. high-risk loans.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* LogisticRegression Model:
  * Balanced Accuracy:  95.2%
  * Precision: Healthy - 1.0, Unhealthy .85
  * Recall: Healthy - .99, Unhealthy, .91

* LogisticRegression Model With Random Oversampling:
  * Balanced Accuracy:  99.3%
  * Precision: Healthy - 1.0, Unhealthy .84
  * Recall: Healthy - .99, Unhealthy, .99

## Summary

In summary, the model shows promise at being able to identify high-risk borrowers.  While additional data and analysis can improve the model, currently, the model has a high recall score for both healthy and high-risk borrowers.  In this application, it is more important to flag individuals who might be high-risk for a loan so that additional screening can be done.  So, the high recall score here suggests that the model is functional and can add an important flag to protect against defaulted loans.