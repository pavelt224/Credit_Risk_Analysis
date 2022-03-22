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

----------------------------------------------------------------------------------------------------------------------------------------------------------------

* Technical Analysis

## RandomOverSampler

![RandomOverSampler_confusion_matrix](https://user-images.githubusercontent.com/93852380/159392148-a63494d9-feab-409a-a081-282d98c49f42.png)


![RamdomOverSampler](https://user-images.githubusercontent.com/93852380/159392160-87e92489-28b5-4de8-b23b-a71909b062ae.png)


## SmoteConfusion

![Smote_confusion_matrix](https://user-images.githubusercontent.com/93852380/159392457-d4f0881b-113c-4dbc-83d6-3b917cffa062.png)


![Smote_confusion](https://user-images.githubusercontent.com/93852380/159392495-4c72d90b-9f0d-45cb-89e1-6104d04e5188.png)

## ClusterCentroids

![ClusterCentroids_confusion_matrix](https://user-images.githubusercontent.com/93852380/159392727-05cded3a-b870-4875-8865-1f2a42d0fb1c.png)


![ClusterCentroids](https://user-images.githubusercontent.com/93852380/159392753-f43973c0-705c-4fae-8507-e4a849eb0f39.png)


## BalancedRandomForestClassifier

![BalancedRandomForestClassifier_confusion_matrix](https://user-images.githubusercontent.com/93852380/159393004-80379a9f-bc76-4ee1-afaa-f4f2b72d437f.png)


![BalancedRandomForestClassifier](https://user-images.githubusercontent.com/93852380/159393017-90d27928-de80-4e04-bacc-8f0862664dad.png)


# Summary
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Given the features used to classify each group of potential loanees, both Ensemble Classifiers and Resampling techniques outperformed the Resampling techniques in accurately predicting high-risk credit card applicants and low-risk applicants, as shown by the summary dataframes and individual model testing. In the case of screening for high-risk individuals, high sensitivity exceeds model precision—it is preferable to limit false negatives and allow those high-risk individuals slide through the cracks undetected in order to safeguard the loaning businesses' interests.

Recommendation Performance based on Model (6) All six models, however, had extremely poor precision scores. In other words, machine learning could only guarantee that those who were designated as high-risk were indeed high-risk 9 percent of the time. With a 91 percent chance of a False Positive result, in which a low-risk applicant is mistaken for a high-risk applicant, I cannot recommend any of the models tested in this project for implementation—regardless of high sensitivity, financial institutions risk losing 91 percent of future customers and revenues of low-risk applicants when they are denied a credit card. Many of these False Positives will file a claim and settle the refused application, but many will take their company elsewhere rather than deal with the hassle of fighting the creditor's decision.



