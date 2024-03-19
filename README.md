# credit-risk-classification


## Overview of the Analysis

Purpose:
The purpose of this analysis is to develop a machine learning algorithm to classify credit risk as either a healthy or high-risk loan. This classification aids companies in assessing the creditworthiness of applicants.

Financial information:
The dataset comprises features such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. These features are utilized to predict whether a loan is classified as healthy or high-risk.

Dataset information(model:1):

For the Total Dataset:

Total number of rows: 77,536

Total number of healthy loans (label 0): 75,036

Total number of high-risk loans (label 1): 2,500


For the Train Data:

Total number of rows: 58,152

Total number of healthy loans (label 0): 56,271

Total number of high-risk loans (label 1): 1,881

For the Test Data:

Total number of rows: 19,384

Total number of healthy loans (label 0): 1,876

Total number of high-risk loans (label 1): 619

Steps:

Load data into a dataframe.

Create loan_status as labels and use the other columns as features.

Split the data into training and test datasets.

Fit a logistic regression model using the training data.

Save the predictions on the testing data labels by using the testing feature data and the fitted model.

Evaluate the model’s performance by generating a confusion matrix and printing the classification report.

Model:
I have used logistic regression model, additionally tested using BalancedRandomForest and Support Vector Machines along with Random over sampler technique.


## Results
logistic regression Model(Model:1):

Accuracy Score:0.99

This indicates  that the model correctly predicts 99% of the loans in the dataset.

## Healthy Loan (0) :

* Precision: 1.00
This means that when the model predicts a loan as healthy, it is 100 % accurate and not wrongly labeled.

* Recall: 0.99
This indicates that the model correctly identifies 99% of all healthy loans in the dataset.

## High-Risk Loan (1):

* Precision: 0.84
This means that when the model predicts a loan as high-risk,it is 84 % accurate and 16% of the time its wrongly labeled. 

* Recall: 0.94
This indicates that the model correctly identifies 99% of all high-risk loans in the dataset.

## Summary
The RandomOverSampler with Logistic Regression model performs better due to its higher accuracy, F1 score, precision, and recall values for both healthy and high-risk loans,along with higher support data for both classes.
I recommend  RandomOverSampler with Logistic Regression model  for credit risk classification to the company.
Yes, the performance of the model depends on the specific problem we are trying to solve. In this case, achieving high precision and recall values for high-risk loans is more significant than for healthy loans.



