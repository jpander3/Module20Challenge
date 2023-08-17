# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

The purpose of this analysis is to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

* Explain what financial information the data was on, and what you needed to predict.

Loan size, interest rate, borrower income, loan status, etc. I was trying to predict the credit risk classifiction of an individual's loan status.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

Loan status of individuals in the dataset are what we want to predict. 0 indicates a healthy loan while 1 indicates a high risk loan. Value_counts tells us that there are 75036 healthy loans and 2500 high risk loans in this dataset.

* Describe the stages of the machine learning process you went through as part of this analysis.

The data was split into training and testing sets using train_test_split. The x and y variables were created, then a logistic regression model was created with the original data and fit using the training data. Predictions were made  and  the models performance was tested by calculating the accuracy score, generating a confusion matrix, and printing a classification report. Finally, a logistic regression model was predicted with resampled training data using the RandomOverSampler module and repeating the previous process using the resampled data.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
The logistic regression module was used to aid predictions. The RandomOverSampler was used to create resampled data.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

  Accuracy: 99%

  Precision: Healthy Loans 100% and the High-Risk Loans 85%. 

  Recall Scores: 99% for Healthy Loans and 91% for High Risk Loans. 


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

  Accuracy: 99%

  Precision: Healthy Loans 100% and the High-Risk Loans 84%. 

  Recall Scores: 99% for Healthy Loans and 99% for High Risk Loans.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?

Machine Learning Model 2 because there was in increase in recall scores for Healthy Loan and High Risk Loans and only a insignificant one percent decrease in only the precisions of High Risk Loans.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

It is more important to predict the '0''s because they carry more weight.

If you do not recommend any of the models, please justify your reasoning.
