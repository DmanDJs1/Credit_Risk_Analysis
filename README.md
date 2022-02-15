# Credit_Risk_Analysis

## Overview

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, 
we oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the 
ClusterCentroids algorithm. Then, we used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 
We then compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, 
to predict credit risk. Once we completed that, we concluded by evaluating the performance of these models and created a written 
recommendation on whether they should be used to predict credit risk.


1. RandomOverSampler model

![image](https://github.com/DmanDJs1/Credit_Risk_Analysis/blob/main/Pictures/RandomOverSampler%20model1.PNG?raw=true)

   - The balanced accuracy score is 66%.
   - The high risk precision is 1% only with a recall of 72% and F1 of only 2% .
   - Its low-risk precision is at 100% with a recall of 60%.

2. SMOTE model

![image](https://github.com/DmanDJs1/Credit_Risk_Analysis/blob/main/Pictures/SMOTE%20Oversampling2.PNG?raw=true)

   - The balanced accuracy score also about 66%.
   - The high-risk precision is about 1% only with 72% recall and F1 of 2% only.
   - Its low-risk precision is 100% with a recall of 60%.

3. Cluster Centroids Undersampling

![image](https://github.com/DmanDJs1/Credit_Risk_Analysis/blob/main/Pictures/Cluster%20Centroids%20Undersampling3.PNG?raw=true)


   - The balanced accuracy score also about 54%.
   - The high-risk precision is 1% only with 69% recall and F1 of 2% only.
   - Its low-risk precision is 100% with a recall of 40%.


4. SMOTEENN Oversampling & Undersampling


![image](https://github.com/DmanDJs1/Credit_Risk_Analysis/blob/main/Pictures/SMOTEOversampling%20-%20Undersampling4.PNG?raw=true)


   - This model's sensitivity towards high risk credits is an improvement over the other models but precision is still very low.

5. Balanced Random Forest Classifier

![image](https://github.com/DmanDJs1/Credit_Risk_Analysis/blob/main/Pictures/Balanced%20Random%20Forest%20Classifier5.PNG?raw=true)

   - We see an a very good increase in the precision but the sensitivity is still very low for high risk credits.

6. Easy Ensemble AdaBoost Classifier

![image](https://github.com/DmanDJs1/Credit_Risk_Analysis/blob/main/Pictures/Easy%20Ensemble%20AdaBoost%20Classifier6.PNG?raw=true)

   - This model gives us the best recall towards high risk credits but only a little increase in precision for high risk credits.

Summary:

Although we have high sensitivity(recall) in our models for High Risk transactions, the precision is very low hence we see a drop in F1 score.

In comparision to all the algorithms, Easy Ensemble AdaBoost Classifier gave the best precision and highest recall for high risk credits. 
Easy Ensemble Classifier is very good if the requirement are to be more sensitive towards high risk transactions. 
Also, if we want high precision for high risk credits, then none of the models shown will be very useful to utilize.
