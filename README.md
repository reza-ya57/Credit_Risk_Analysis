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

By checking the different method that we used to build a model, random over sampling, smote and undersampling method is not recomend as a method for sammpling for this dataset as they are working on the actual data from the real users to build a training data. You can see the accuracy of these models which are below than 67%.
In the other hand by using balanced random forest and ensemble adaboost classifier our model can create more data to increase the accuracy and help balance of sampling. So I recomend using AdaBoost Classifier or Balanced Random Forest Classifier to build a model for this dataset. Adaboost Classifier is the best one based on the result that is mentioned in above. 


