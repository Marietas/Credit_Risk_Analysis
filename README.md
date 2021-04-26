# Credit_Risk_Analysis

## Overview

The propose of this project is to apply machine learning to solve a real-world challenge to predict credit risk.
To develop this analysis we have to use different techniques to evaluate models with unbalanced classes. Therefore the following models were applied for this analysis:

 - RandomOverSampler and SMOTE algorithms; 
 - ClusterCentroids algorithm;
 - SMOTEENN algorithm; 
 - And finally the BalancedRandomForestClassifier and EasyEnsembleClassifier.
 
Imbalanced-learn and scikit-learn libraries have been applied to build and evaluate models. The final result is to present the performance of these models to check whether they should be used to predict credit risk.

### Resources
- Phyton with Machine learning module
- Dataset LoanStats_2019Q1.CSV

## Results

- RandomOverSampler Model

![image](https://user-images.githubusercontent.com/76540704/116019863-2d53fb00-a613-11eb-960a-d83e1662b708.png)

- SMOTE Model

![image](https://user-images.githubusercontent.com/76540704/116020168-c3882100-a613-11eb-80da-5185c0f201e2.png)

- ClusterCentroids Model

![image](https://user-images.githubusercontent.com/76540704/116020703-d9e2ac80-a614-11eb-86e1-cc92fbc8f01c.png)

- SMOTEENN model

![image](https://user-images.githubusercontent.com/76540704/116021080-7907a400-a615-11eb-8cb7-57b4089a1c14.png)


- Balanced Random Forest Classifier model

![image](https://user-images.githubusercontent.com/76540704/116021631-90935c80-a616-11eb-92d3-42406adb1613.png)

- EasyEnsembleClassifier

![image](https://user-images.githubusercontent.com/76540704/116021915-2f1fbd80-a617-11eb-8c7e-70d9c43bf84a.png)

## Summary

This project is designed to identify the suitable model that can inform whether a loan is high risk or not. As a result, we need to develop a model that allows the least amount of high-risk loans to move unnoticed. The recall rate for high risk is the corresponding metric for this. The following versions received the best scores as compared to the others:

1. Easy Ensemble Classifying - 92.5%
2. SMOTEENN Sampling - 61.91%
3. Naive Random Oversampling - 66.73%

Although this is the most interesting statistic from this study, recall rate for low risk loans is also important since it indicates how many low risk loans are flagged as high risk. The following versions received the best scores as compared to the others:

- Balanced Random Forest Classifying - 78.77%
- Easy Ensemble Classifying - 92.54%

We should look at the accurary score after we've weighed these two numbers against the others and get a sense of how well the model does in general. The following versions have the best accuracy scores:

- Easy Ensemble Classify (92.3%)
- SMOTEENN Sampling (68.1%)
- Balanced Random Forest Classifying (64.8%)

The Easy Ensemble Classifying model is the model that I would prefer for forecasting high risk loans after factoring in these three major statistics.


