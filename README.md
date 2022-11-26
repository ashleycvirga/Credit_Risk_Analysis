# Credit_Risk_Analysis

Using Python to evaluate multiple machine learning models that predict credit risk.

## Overview

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.  This project employs different techniques to train and evaluate Machine Learning models with unbalanced classes. Imbalanced-learn and scikit-learn libraries in Python were utilized to build and evaluate multiple Machine Learning models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, this project oversampled the data using the RandomOverSampler(1) and SMOTE(2) algorithms and undersampled the data using the ClusterCentroids(3) algorithm. 

Then, it uses a combinatorial approach of over- and undersampling using the SMOTEENN(4) algorithm.

Finally, the project compares two new machine learning models that reduce bias, BalancedRandomForestClassifier(5) and EasyEnsembleClassifier(6), to predict credit risk. 

Which ML model performs best at accurately predicting credit risk?

## Results

1. RandomOverSampler

![random_oversampling](https://github.com/ashleycvirga/Credit_Risk_Analysis/blob/1dc1b57c142aa3a2dfdbb218e3965869f283d91c/Resources/random_oversampling.png)

 - Balanced Accuracy Score: 0.657 (65.7%)

 - High-Risk Precision: 0.01

 - Low-Risk Precision: 1.00

 - High-Risk Recall/Sensitivity: 0.71

 - Low-Risk Recall/Sensitivity: 0.60



2. SMOTE

![SMOTE](https://github.com/ashleycvirga/Credit_Risk_Analysis/blob/1dc1b57c142aa3a2dfdbb218e3965869f283d91c/Resources/SMOTE.png)

 - Balanced Accuracy Score: 0.662 (66.2%)

 - High-Risk Precision: 0.01

 - Low-Risk Precision: 1.00

 - High-Risk Recall/Sensitivity: 0.63

 - Low-Risk Recall/Sensitivity: 0.69




3. ClusterCentroids

![ClusterCentroids](https://github.com/ashleycvirga/Credit_Risk_Analysis/blob/1dc1b57c142aa3a2dfdbb218e3965869f283d91c/Resources/ClusterCentroids.png)

 - Balanced Accuracy Score: 0.5447 (54.5%)

 - High-Risk Precision: 0.01

 - Low-Risk Precision: 1.00

 - High-Risk Recall/Sensitivity: 0.69

 - Low-Risk Recall/Sensitivity: 0.40




4. SMOTEENN

![SMOTEENN](https://github.com/ashleycvirga/Credit_Risk_Analysis/blob/1dc1b57c142aa3a2dfdbb218e3965869f283d91c/Resources/SMOTEENN.png)
 
 - Balanced Accuracy Score: 0.6447 (64.5%)

 - High-Risk Precision: 0.01

 - Low-Risk Precision: 1.00

 - High-Risk Recall/Sensitivity: 0.72

 - Low-Risk Recall/Sensitivity: 0.57




5. BalancedRandomForestClassifier

![]()

 - Balanced Accuracy: 

 - High-Risk Precision:

 - Low-Risk Precision: 

 - High-Risk Recall/Sensitivity: 

 - Low-Risk Recall/Sensitivity: 




6. EasyEnsembleClassifier

![]()

 - Balanced Accuracy: 

 - High-Risk Precision:

 - Low-Risk Precision: 

 - High-Risk Recall/Sensitivity: 

 - Low-Risk Recall/Sensitivity: 




## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

