# Credit_Risk_Analysis

Using Python to evaluate multiple machine learning models that predict credit risk.

## Overview

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.  This project employs different techniques to train and evaluate Machine Learning models with unbalanced classes. Imbalanced-learn and scikit-learn libraries in Python were utilized to build and evaluate multiple Machine Learning models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, this project oversampled the data using the RandomOverSampler(1) and SMOTE(2) algorithms and undersampled the data using the ClusterCentroids(3) algorithm. 

Then, it uses a combinatorial approach of over- and undersampling using the SMOTEENN(4) algorithm.

Finally, the project compares two new machine learning models that reduce bias, BalancedRandomForestClassifier(5) and EasyEnsembleClassifier(6), to predict credit risk. 

Which ML model performs best at accurately predicting credit risk?

## Results

### 1. RandomOverSampler

![random_oversampling](https://github.com/ashleycvirga/Credit_Risk_Analysis/blob/1dc1b57c142aa3a2dfdbb218e3965869f283d91c/Resources/random_oversampling.png)

 - Balanced Accuracy Score: 0.657 (65.7%)

 - High-Risk Precision: 0.01

 - Low-Risk Precision: 1.00

 - High-Risk Recall/Sensitivity: 0.71

 - Low-Risk Recall/Sensitivity: 0.60



### 2. SMOTE

![SMOTE](https://github.com/ashleycvirga/Credit_Risk_Analysis/blob/1dc1b57c142aa3a2dfdbb218e3965869f283d91c/Resources/SMOTE.png)

 - Balanced Accuracy Score: 0.662 (66.2%)

 - High-Risk Precision: 0.01

 - Low-Risk Precision: 1.00

 - High-Risk Recall/Sensitivity: 0.63

 - Low-Risk Recall/Sensitivity: 0.69




### 3. ClusterCentroids

![ClusterCentroids](https://github.com/ashleycvirga/Credit_Risk_Analysis/blob/1dc1b57c142aa3a2dfdbb218e3965869f283d91c/Resources/ClusterCentroids.png)

 - Balanced Accuracy Score: 0.5447 (54.5%)

 - High-Risk Precision: 0.01

 - Low-Risk Precision: 1.00

 - High-Risk Recall/Sensitivity: 0.69

 - Low-Risk Recall/Sensitivity: 0.40




### 4. SMOTEENN

![SMOTEENN](https://github.com/ashleycvirga/Credit_Risk_Analysis/blob/1dc1b57c142aa3a2dfdbb218e3965869f283d91c/Resources/SMOTEENN.png)
 
 - Balanced Accuracy Score: 0.6447 (64.5%)

 - High-Risk Precision: 0.01

 - Low-Risk Precision: 1.00

 - High-Risk Recall/Sensitivity: 0.72

 - Low-Risk Recall/Sensitivity: 0.57




### 5. BalancedRandomForestClassifier

![brf_model](https://github.com/ashleycvirga/Credit_Risk_Analysis/blob/5513433d471f71bbd9a651d206d988a2f55ea236/Resources/brf_model.png)

 - Balanced Accuracy Score: 0.7877 (78.8%)

 - High-Risk Precision: 0.04

 - Low-Risk Precision: 1.00

 - High-Risk Recall/Sensitivity: 0.67

 - Low-Risk Recall/Sensitivity: 0.91




### 6. EasyEnsembleClassifier

![eec_model](https://github.com/ashleycvirga/Credit_Risk_Analysis/blob/5513433d471f71bbd9a651d206d988a2f55ea236/Resources/eec_model.png)

 - Balanced Accuracy Score: 0.925 (92.5%) !!!

 - High-Risk Precision: 0.07

 - Low-Risk Precision: 1.00

 - High-Risk Recall/Sensitivity: 0.91

 - Low-Risk Recall/Sensitivity: 0.94




## Summary

Overall, the majority of the models did not have very good balanced accuracy scores. The EasyEnsembleClassifier model was able to achieve the highest balanced accuuracy score of 92.5%.  This means that the model has a 92.5% chance of correctly predicting loan_status.

The precision scores for predicting 'high-risk' loan_status was incredibly low for all of the models tested.  On the contrary, the precision scores for predicting 'low-risk' loan_status was 100% for every single model.  High precision for low risk loan status means that if the test comes back positive for being low risk, there's a high likelihood that the loan status is in fact a low risk loan.  

The recall/sensitivity scores were tetering in the midranges for the majority of the models.  The EasyEnsembleClassifier model shined through again though with the highest recall/sensitivity score of them all.  The EasyEnsembleClassifier model was able to predicting both high-risk and low-risk loan status with above 90% recall/sensitivity.  Luckily in this case, recall/sensitivity scores are more important than precision scores when predicting loan status. It is important to use a model wwith a strong sensitivity for predicting high-risk loans to notify lenders of all possible loans that may be high-risk, even if a small percentage of those identified as high risk may not actually be high risk loans. The alternative is that the model has a high sensitivity for predicting low risk loans.  This case would more often misidentify high risk loans as low risk and could end up costing the lender large sums of money due to default.

The EasyEnsembleClassifier model seems to win out amongst the 6 models tested in this project! When predicting loan status, it is important to use a model with high sensitivity for predicting high-risk loans so that loaners can be aware of all loans that may be high-risk, even if some of them may be falsely predicted with that status.
