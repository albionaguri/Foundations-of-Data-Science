# Loan-Approval-Prediction
## Business Problem Statement

Automating the loan qualification process is the primary goal of this project. A decision-making method called predict loan approval uses applicant data to decide whether or not a potential borrower is qualified for a loan.

## Introduction

Many people are seeking for bank loans as a result of the expansion of the banking industry, but because banks only have a certain amount of assets they can lend to, it is safer for them to find out who they can lend to. We created a machine learning model to anticipate loan acceptance in order to automate the loan qualification process.

## Used Libraries and Resources

Python Version : 3.6

Libraries : sklearn, pandas, numpy, matplotlib, seaborn

## Data Preprocessing

* Based on domain knowledge I removed columns which are not relevant for prediction.
* Handling missing and unwanted/strange values in the features.
* Encoding categorical features.
* Feature Selection using Recursive Elemination with cross validation.

## Models

The problem is a binary classification and different machine learning models were used:

● Logistic Regression

● Support Vector Classification (SVC)

● Gaussian Naive Bayes (GaussianNB)

● K-Nearest Neighbors (KNeighborsClassifier)

● Linear Discriminant Analysis (LinearDiscriminantAnalysis)

## Benchmark

<img width="372" alt="image" src="https://user-images.githubusercontent.com/51866742/235441702-dc60e8f3-62d7-49d9-be3b-9d839f7fd97e.png">

## Future Scope

* Use additional ML estimators
* To possibly improve model performance, explore other methods for handling unbalanced data.

## Conclusion

SVC and KNN are not the appropriate models for the problem when one considers the fact that we used Precision as the primary metric, that these models do not perform well on unbalanced data, and that our dataset is unbalanced.The AUC score metric was the main focus since it is preferable to find a model that works well in both minority and majority classes rather than only in the majority class.The optimal model would be logistic regression because it has the highest AUC score in an unbalanced dataset, as well as the maximum precision, recall, and f1-score for each class.
An issue with binary classification exists. The objective is to identify those who shouldn't be granted a loan in the right way. The F1-score and the AUC score are therefore given the most attention.
