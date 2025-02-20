# Challenge 20: Credit Risk Classification
This repo contains code and analysis for the Module 20 Challenge. Code for this challenge can be found in Credit_Risk/credit_risk_classification.ipynb. The analysis component can be found below. Refernces for this work can be found in the 'References' section below.


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
Overall, the logistic regression model trained on the loan profile data performs well when predicting whether a loan profile is healthy or high risk, based on a range of loan features. 

If used to classify loan customers, this model can be recommended for use, based on high scores for accuracy, precision and recall. In general, the model produced accurate classifications, and is appropriate for use.

Two scenarios to consider:
1) The model's weakness is incorrectly classifying healthy profiles as high-risk. In practice, there is limited risk to the loan issuer, as cases of misclasification of healthy profiles as high-risk would trigger additional review of a profile prior to any further action.
2) A potentially problematic scenario is the classification of high-risk profiles as healthy. In this scenario, high-risk borrowers may be allowed to gain access to additional credit without additional review. That said, the model successfully minimizes this scenario, scoring 0.98 for recall with high-risk profiles. Out of 619 high-risk profiles in the test data, only 10 were incorrectly classified as healthy. 


## References
References for this project are listed here. The number associated with each refernce corresponds to the reference numbers included in code comments.

1) https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html
2) Module 20; Lesson 1; Acivity 3; logistic_regression_solution.ipynb
3) https://scikit-learn.org/stable/modules/generated/sklearn.metrics.confusion_matrix.html#sklearn.metrics.confusion_matrix
4) https://scikit-learn.org/stable/modules/generated/sklearn.metrics.classification_report.html









