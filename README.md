# Credit_Risk_Analysis
## Overview of the Study

### In this project by using machine learning technique we try to build a model to predict the credit risk for a peer to peer lending services company.
#### Due to nature of the credit risk, it categorized as a unbalanced classification problem, so we used resampling technique to build and evaluate models. Below are two libraries that we used for this project
- imbalanced-lean
- scikit-learn

### Methods and techniques that we used in this study are as below
#### We used two below algorithms to oversample the data:
- RandomOverSampler
- SMOTE
##### We also used undersampling teqniques by using below algorithm
- ClusterCentroids
#### To make examin the best method for model this problem we also used a combination method of over- and undersampling by using below algorithm:
- SMOTEENN
#### And finaly we compare two new machine learning models that reduce bias to predict credit risk.
- BalancedRandomForestClassifier
- EasyEnsembleClassifier

## Result
### Random Oversampling Result
- Balance Accuracy Score = 0.67

![total_review](https://github.com/reza-ya57/Credit_Risk_Analysis/blob/main/Images/RandomOverSampling.png)

### SMOTE Oversampling
- Balance Accuracy Score = 0.66
![total_review](https://github.com/reza-ya57/Credit_Risk_Analysis/blob/main/Images/SMOT.png)

### ClusterCentroids
- Balance Accuracy Score = 0.54

![total_review](https://github.com/reza-ya57/Credit_Risk_Analysis/blob/main/Images/Undersampling.png)

### SMOTEENN
- Balance Accuracy Score = 0.64

![total_review](https://github.com/reza-ya57/Credit_Risk_Analysis/blob/main/Images/SMOTEENN.png)

### Balanced Random Forest Classifier
- Balance Accuracy Score = 0.77

![total_review](https://github.com/reza-ya57/Credit_Risk_Analysis/blob/main/Images/BRF.png)

### AdaBoost Classifier
- Balance Accuracy Score = 0.93

![total_review](https://github.com/reza-ya57/Credit_Risk_Analysis/blob/main/Images/AdaBoost.png)


## Summary

With comparing the Accuracy Score among different model that I used for this study, AdaBoost Classifier has the highest accuracy score. On the other hand precision for predicting the high risk credit is not good also recall score has a good result. 
In summary I can say this model has a imbalance sensitivity and precision as we can also see in f1 score which is low, so I dont recomend this model for predicting the credit risk. 

