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

![total_review](https://github.com/reza-ya57/Amazon_Vine_Analysis/blob/main/total_review_paid_unpaid.png)

### SMOTE Oversampling
- Balance Accuracy Score = 0.66
- image

### ClusterCentroids
- Balance Accuracy Score = 0.54
- image

### SMOTEENN
- Balance Accuracy Score = 0.64
- image

### Balanced Random Forest Classifier
- Balance Accuracy Score = 0.77
- image

### AdaBoost Classifier
- Balance Accuracy Score = 0.93
- image


### What is Vine program?
#### The Amazon Vine Program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
# Goal of this study
## Identify any positivity bias for reviews in the vine program. To cover this goal we are going to answer below question:
### How many Vine reviews and non-Vine reviews were there?
- Vine reviews: There were 579 Vine reviews in total for this study
- non_Vine reviews: There were 47521 non-Vine reviews in total for this study

![total_review](https://github.com/reza-ya57/Amazon_Vine_Analysis/blob/main/total_review_paid_unpaid.png)
### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- Vine reviews: Totaly there were 246 reviews with 5-star rating in Vine program

![5_star_vine_review](https://github.com/reza-ya57/Amazon_Vine_Analysis/blob/main/total_review_paid_5_star.png)
- non-Vine reviews: Totaly there were 23816 reviews with 5-star rating in non-Vine program

![5_star_non_vine_review](https://github.com/reza-ya57/Amazon_Vine_Analysis/blob/main/total_review_unpaid_5_star.png)
- Also in case that you want to comare the other grade of reviews you can check below tables which are show the total number of review per each rating star for each Vine and non-Vine program.

![total_review_per_star-paid](https://github.com/reza-ya57/Amazon_Vine_Analysis/blob/main/total_review_paid_per_star.png)
![total_review_per_star-unpaid](https://github.com/reza-ya57/Amazon_Vine_Analysis/blob/main/total_review_unpaid_per_star.png)
### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- Vine program: In vine program almost 42% of the reviews are 5-star
- non-Vine program: In non-vine program almost 50% of the review are 5 star

![5_star_percentage](https://github.com/reza-ya57/Amazon_Vine_Analysis/blob/main/5_star_percent.png)

## Summary
### By looking at the difference of 5-star review percentage between vine program and none-vine program we can say there is almost 8% negative bias in vine program for 5-star rating.<br> It is note a big difference but vine program would be more accurate and it should be worth for company to use this program for getting more accurate feedback from the customer. <br>
### By comparing the 1-star rating in both vine and none-vine program we can see more gap between these to program. The difference is about 10% so we can assume people in vine program write the review more accurate. 
