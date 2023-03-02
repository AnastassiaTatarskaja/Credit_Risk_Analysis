# Credit_Risk_Analysis

## Overview of the Analysis:

Since good loans easily outnumber risky loans, calculating credit risk becomes an unbalanced classification problem. Different techniques were used to train and evaluate models with unbalanced classes. imbalanced-learn and scikit-learn libraries were used to build and evaluate models using resampling.

Using the credit card dataset from LendingClub, a peer-to-peer lending services company,  the data was oversampled using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm was used. Next, two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk were used. Finally, the performance of these models was evaluated and a written recommendation was made on whether they should be used to predict credit risk.

## Results:

### Naive Random Oversampler

- precision 0.99
- recall 0.68
- balanced accuracy 0.42

![image](https://user-images.githubusercontent.com/107759305/222335951-d5c06a77-adc6-4845-98f8-b5ed4628611c.png)

### SMOTE

- precision 0.99
- recall 0.67
- balanced accuracy 0.40

![image](https://user-images.githubusercontent.com/107759305/222336115-7af3f911-05e4-4b0a-b379-21316eff1a3f.png)

### Cluster Centroids

- precision 0.99
- recall 0.46
- balanced accuracy 0.27

![image](https://user-images.githubusercontent.com/107759305/222336226-79685388-a305-4469-8fc7-7b7dd5c03ac4.png)

### SMOTEENN

- precision 0.99
- recall 0.55
- balanced accuracy 0.36

![image](https://user-images.githubusercontent.com/107759305/222336340-40f10765-1459-4d4e-9864-901cffcdbe8a.png)

### Balanced Random Forest Classifier

- precision 0.99
- recall 0.94
- balanced accuracy 0.86

![image](https://user-images.githubusercontent.com/107759305/222336445-59c6eaf4-a1db-42d7-ada3-3cff824036a4.png)

### Easy Ensemble AdaBoost Classifier

- precision 0.99
- recall 0.94
- balanced accuracy 0.86

![image](https://user-images.githubusercontent.com/107759305/222336533-b1e17c65-01e6-4512-a7f9-421b4aeb0243.png)

## Summary:

When looking at all six models, Easy Ensemble AdaBoost Classifier performs the most effective. It provides the highest score for all risk models. Based on the above statement, we can conclude that we should move forward with this estimator for further predictions.

The highest score for predicting both low-risk and high risk loan statuses was found in The Oversampling Recall Score (with SMOTE) machine learning model. We can conclude that it is the best model considering the financial cost risk associated with False Negatives.




















