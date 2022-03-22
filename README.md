# Credit_Risk_Analysis

## Data Preparation, Statistical Reasoning and Machine Learning: Predicting Credit Card Risk

Challenge Overview

This project's goal is to use supervised machine learning algorithms to assess credit card risk. To ensure low default, financial institutions, banks, and peer-to-peer lending organizations should automate and increase the accuracy of spotting high-risk individuals prior to giving loans. Machine learning is particularly difficult due to the unequal distribution of risk classification (low risk vs high risk), as there are significantly more low-risk applicants than low-risk applicants in any given sample dataset.

Due to the difficulties of screening for fewer high-risk applicants, it is beneficial to use a variety of machine learning models to eliminate bias and resample datasets in order to find the optimal methodology or algorithm for properly predicting credit-card risk. We look at six different models.

## Features and Data Resources

* Data Source: LoanStats_2019Q1.csv
* Data Tools: credit_risk_resampling.ipynb and credit_risk_emsembler.ipynb
* Software: imbalanced-learn, skikit-learn, Jupyter Notebook and Python.9.2.3

# Results

* Resampling Machine Learning

![SMOTEENN_confusion_matrix](https://user-images.githubusercontent.com/93852380/159374689-4ab0e707-ed87-4464-a83d-b7225d68b112.png)


![CreditRiskResampling](https://user-images.githubusercontent.com/93852380/159374553-ee39438d-ff9b-4955-b2f4-b73a865772e7.png)




* Ensemble Classifers

![EasyEnsembleClassifier_confusion_matrix](https://user-images.githubusercontent.com/93852380/159374981-b992aaae-96b6-4d6a-bda8-6de031ec9048.png)


![imbalanced classification report(ensemble)](https://user-images.githubusercontent.com/93852380/159374896-11fd6fee-2488-4bc4-8c01-2fea211f7460.png)



# Top ML Models: Performance Metrics
* Best Overall Balanced Accuracy Score: Easy Ensemble Classifer (93%)
* Best Overall Precision: Easy Ensemble Classifer (9%)
* Best Overall Recall: Easy Ensemble Classifer (92%)
