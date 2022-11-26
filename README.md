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

![]()

 - Accuracy: 

 - Precision (High-Risk):

 - Precision (Low-Risk): 

 - Sensitivity (High-Risk): 

 - Sensitivity (Low-Risk): 



2. SMOTE

![]()

- Accuracy: 

- Precision (High-Risk): 

- Precision (Low-Risk): 

- Sensitivity (High-Risk): 

- Sensitivity (Low-Risk): 



3. ClusterCentroids

![]()

- Accuracy: 

- Precision (High-Risk): 

- Precision (Low-Risk): 

- Sensitivity (High-Risk): 

- Sensitivity (Low-Risk): 



4. SMOTEENN

![]()

- Accuracy: 

- Precision (High-Risk): 

- Precision (Low-Risk): 

- Sensitivity (High-Risk): 

- Sensitivity (Low-Risk): 



5. BalancedRandomForestClassifier

![]()

- Accuracy: 

- Precision (High-Risk): 

- Precision (Low-Risk): 

- Sensitivity (High-Risk): 

- Sensitivity (Low-Risk): 



6. EasyEnsembleClassifier

![]()

- Accuracy: 

- Precision (High-Risk): 

- Precision (Low-Risk): 

- Sensitivity (High-Risk): 

- Sensitivity (Low-Risk): 



## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

