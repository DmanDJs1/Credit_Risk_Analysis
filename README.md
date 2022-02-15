# Credit_Risk_Analysis

## Overview

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, 
we will need to oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the 
ClusterCentroids algorithm. Then, we will need to use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 
We will then compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, 
to predict credit risk. Once we have completed that, we will conclude by evaluating the performance of these models and make a written 
recommendation on whether they should be used to predict credit risk.


1. RandomOverSampler model

![image](https://github.com/DmanDJs1/Credit_Risk_Analysis/blob/main/Pictures/RandomOverSampler%20model1.PNG?raw=true)

    - The balanced accuracy score is about 65%.
    - The high risk precision is about 1% only with a recall of 69% and F1 of only 2% .
    - Its low-risk precision is almost at 100% with a recall of 59%.

2. SMOTE model

![image](https://github.com/DmanDJs1/Credit_Risk_Analysis/blob/main/Pictures/SMOTE%20Oversampling2.PNG?raw=true)

    - The balanced accuracy score also about 65%.
    - The high-risk precision is about 1% only with 69% recall and F1 of 2% only.
    - Its low-risk precision is almost 100% with a recall of 59%.

3. Cluster Centroids Undersampling

![image](https://github.com/DmanDJs1/Credit_Risk_Analysis/blob/main/Pictures/Cluster%20Centroids%20Undersampling3.PNG?raw=true)


   - This model gives us very low recall as well as precision for high risk transactions.

4. SMOTEENN Oversampling & Undersampling


![image](https://github.com/DmanDJs1/Credit_Risk_Analysis/blob/main/Pictures/SMOTEOversampling%20-%20Undersampling4.PNG?raw=true)


    - This model's sensitivity towards high risk credits is a little better than other models but precision is still very low.

5. Balanced Random Forest Classifier

![image] ( )

    - We see a slight increase in precision but sensitivity is still very low for high risk credits.

6. Easy Ensemble AdaBoost Classifier

![image] ( )

    - This model is by far giving us the best recall towards high risk credits. There is a little increase in precision as well for high risk credits.

Summary:

Although we have high sensitivity(recall) in our models for High Risk transactions but precision is very low hence we see a drop in F1 score.

In comparision to all the algorithms, Easy Ensemble Classifier gave the best precision and highest recall for high risk credits. 
Easy Ensemble Classifier is very good if the requirement are to be more sensitive towards high risk transactions. 
Also, if we want high precision for high risk credits, then none of the models shown will be very useful to utilize.
