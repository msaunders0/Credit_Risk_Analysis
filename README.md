# Credit_Risk_Analysis

## Overview

For this project, a credit card credit dataset provided by LendingClub (a peer-to-peer lending services company) has beeen used to measure, analyze, and predict credit risk. The data has been oversampled using the RandomOverSampler and SMOTE algorithms and undersampled using the ClusterCentroid algorithm, as well as a combined over and undersampling approach through the SMOTEENN algorithm. The BalancedRandomForestClassifier and EasyEsnembleClassifier machine learning models have then been applied to reduce bias and make predictions.

## Purpose

The purpose of this project is to explore some of the sampling methods and machine learning models from the imbalanced-learn and scikit-learn libraries in order to evaluate and predict credit risk.

## Results

### Native Random Oversampling:
![image](https://github.com/msaunders0/Credit_Risk_Analysis/blob/main/Resources/native_over.png)

### SMOTE Oversampling:
![image](https://github.com/msaunders0/Credit_Risk_Analysis/blob/main/Resources/smote_over.png)

### ClusterCentroids Undersampling:
![image](https://github.com/msaunders0/Credit_Risk_Analysis/blob/main/Resources/cc_under.png)

### SMOTEENN Combined Over and Undersampling:
![image](https://github.com/msaunders0/Credit_Risk_Analysis/blob/main/Resources/smoteenn_combined.png)

### BalancedRandomForestClassifier Ensemble:
![image](https://github.com/msaunders0/Credit_Risk_Analysis/blob/main/Resources/brfc_ensemble.png)

### EasyEnsembleClassifier Ensemble:
![image](https://github.com/msaunders0/Credit_Risk_Analysis/blob/main/Resources/eec_ensemble.png)

## Summary

Overall, the goal was to determine which model was the most useful in predicting credit risk for a loan. Based on the results, it appears as though the ensemble classifier models produced a significantly higher accuracy, precision, and recall scores compared to the rest of the models. Accordingly, these results suggest that using the BalancedRandomForestClassifier and EasyEnsembleClassifier are more accurate and useful for predicting credit risk than the other models, atleast on this specific dataset.

Furthermore, while the scores for the ensemble models are higher, precision is still relatively low, with the EasyEnsembleClassifier producing the highest precision score of the group with 7% for high risk. This would still create an unfortunate circumstance where many false positives are being flagged in the high risk category, which will affect low risk individuals by inaccurately flagging them as high risk. Therefore, my recommendation would be to explore the use of other models in order to flag potential borrowers more accurately.
