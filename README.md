# Credit_Risk_Analysis

## Overview of the Analysis

The purpose of the analysis is to implement machine learning techniques to do classification of credit risk dataset.Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore,different techniques has to be used to train and evaluate models with unbalanced classes.

Analysis is done on the credit card credit dataset from LendingClub, a peer-to-peer lending services companydataset: -https://github.com/merinanto/Credit_Risk_Analysis/blob/main/LoanStats_2019Q1.zip

## Results

### Scripts  Used for Analysis

1.Resampling models is implemented using the script :- https://github.com/merinanto/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb

 - Logistic Regression Model applied on RandomOversampler Data SCORES 
![image](https://github.com/merinanto/Credit_Risk_Analysis/blob/main/Resources/Overresampledlgfs.png) 

 - Logistic Regression Model applied on SMOTE Data SCORES
![image](https://github.com/merinanto/Credit_Risk_Analysis/blob/main/Resources/SMOTEOversampleddata.png)

 - Logistic Regression Model applied on ClusterCentroids resampler Data SCORES
![image](https://github.com/merinanto/Credit_Risk_Analysis/blob/main/Resources/Undersampleddata.png)

 - Logistic Regression Model applied on SMOTEENN Sampled Data SCORES
![image](https://github.com/merinanto/Credit_Risk_Analysis/blob/main/Resources/SMOTEENNSampledData.png)

2.Ensemble Classifiers is  implemented using the script :- https://github.com/merinanto/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb

- BalancedRandomForestClassifier Algorithm SCORES 
 ![image](https://github.com/merinanto/Credit_Risk_Analysis/blob/main/Resources/BalRndmfrstClassifer.png)
 
  - Features sorted in desc order
   ![image](https://github.com/merinanto/Credit_Risk_Analysis/blob/main/Resources/BalRndmfrstClassiferImp.png)

 - EasyEnsembleClassifier Algorithm SCORES
 ![image](https://github.com/merinanto/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifier.png)
 
 ### Analysis
 
 1.In the resampled data ,Accuracy score  for RandomOverSampler -66% SMOTEENN  -65%, SMOTE  -62% & Under sampled data -53%.
   Also looking through classification report and confusion matrix ,Random sampler is having most favourable in resampling data
 
 2.In Ensemble classifiers Accuracy score  Balanced Random Classifier -71%,EasyEnsembleClassifier - 93%
   Also looking through classification report and confusion matrix ,EasyEnsembleClassifier is having more  favourable scores.
 
 3.Overall EasyEnsembleClassifier looks like best supervised ML technique for CreditRisk Analysis.
 
 ## Summary
 
 Analysing through different Supervised ML  techniques EasyEnsembleClassifier is best algorithm that can be used for CreditRisk Analysis 
 as due below reasons
 
 - High Balanced Accuracy SCORE
 - very small error true & error false predictions
 - Overall ver good classification report scores



