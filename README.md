# credit-risk-classification
This repo contains code and analysis for the Module 20 Challenge.


## Credit Risk Analysis Report

### Overview of the Analysis

The purpose of this analysis is to develop a logistic regression model, which can be used to predict whether a loan profile is healthy or high risk.

The model developed for this analysis was trained on loan profile features, which included loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks and total debt.

The loan data was split into training and test data, with 75% of data used for training the model and 25% for testing the model. Additionally, the training data was scaled to improve the model's performance.

A confusion matrix and classification report were genearted to evaluate the performance of the model.



### Results
* Accuracy:
    * The model has a 0.99 accuracy score, meaning that the model was highly successful at correctly predicting whether a loan profile was healthy or high risk.
* Precision:
    * Healthy Loans ('Class 0'): The model gets a 1.00 score for precision. The model was extremely successful at correctly classifying healthy loan profiles, with limited instances of high-risk profiles being classified has healthy.
    * High-risk loans ('Class 1'): The model gets a 0.84 score for precision. There were a noteable number of instances where healthy profiles were incorrectly classified as high risk.
* Recall:
    * Healthy Loans ('Class 0'): The model gets a 0.99 recall score. Approximaly 99% of healthy profiles were correctly classified as healthy, whereas approximately 1% of healthy profiles were incorrectly classified as high-risk.
    * High-Risk Loans ('Class 1'): The model gets a 0.98 reacll score. Approximately 98% of high-risk profiles were correctly classified as high-risk, whereas approximately 2% of high-risk profiles were incorrectly classified as healthy.

### Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
