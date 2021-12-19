# Credit_Risk_Analysis
# Project Overview
This project focuses on how to apply machine learning to solve a real-world challenge: credit card risk.
Credit risk is considered to be an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, different techniques will be employed to train and evaluate models with unbalanced classes.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, one will oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm will be used. Next, one will compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Afterwards, the performance of these models will be evaluated and one will make a written recommendation on whether they should be used to predict credit risk.

# Deliverable 1: Use Resampling Models to Predict Credit Risk

Using the knowledge of the imbalanced-learn and scikit-learn libraries, one will evaluate three machine learning models by using resampling to determine which is better at predicting credit risk. First, one will use the oversampling "RandomOverSampler" and "SMOTE" algorithms, and then use the undersampling "ClusterCentroids" algorithm. Using these algorithms, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.
# RandomOverSampler
![image](https://user-images.githubusercontent.com/89113627/146693115-66dc118f-bb00-4c49-99ea-a20efeda059e.png)
![image](https://user-images.githubusercontent.com/89113627/146693161-c8a1ac50-f805-43aa-8be6-8847afa92ee7.png)
# SMOTE
![image](https://user-images.githubusercontent.com/89113627/146693348-4d488206-5ae7-413c-9832-3d8567ebb640.png)
![image](https://user-images.githubusercontent.com/89113627/146693379-c453286b-2c67-40f3-ba72-f5c896d1cdd1.png)
# ClusterCentroids
![image](https://user-images.githubusercontent.com/89113627/146693477-8da122ee-474d-478a-9872-a16681a06619.png)
![image](https://user-images.githubusercontent.com/89113627/146693524-e32adea8-5486-4dd0-8822-4bfc203d7092.png)

# Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk

Using the knowledge of the imbalanced-learn and scikit-learn libraries, a combinatorial approach of over- and undersampling with the SMOTEENN algorithm are being used to determine if the results from the combinatorial approach are better at predicting credit risk than the resampling algorithms from Deliverable 1. Using the SMOTEENN algorithm, there is need to resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.
# SMOTEENN algorithm: combination over and under-sampling
![image](https://user-images.githubusercontent.com/89113627/146693724-c744342d-5d0d-49b4-becd-dc10e3dd025b.png)
![image](https://user-images.githubusercontent.com/89113627/146693766-1c1e2753-b77a-4ad1-9806-e1a02e97c890.png)

# Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

Using the knowledge of the "imblearn.ensemble" library, train and compare two different ensemble classifiers: "BalancedRandomForestClassifier" and "EasyEnsembleClassifier" to predict credit risk and evaluate each model. Using both algorithms, resample the dataset, view the count of the target classes, train the ensemble classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.
# BalancedRandomForestClassifier
![image](https://user-images.githubusercontent.com/89113627/146693975-fd987d95-1000-4ee8-a384-ccf82738c8f2.png)
![image](https://user-images.githubusercontent.com/89113627/146693995-28fa6016-7fb8-4c74-938d-c27c67f62db2.png)
# EasyEnsembleClassifier
![image](https://user-images.githubusercontent.com/89113627/146694061-d2d3419e-579d-43ee-9da8-62c2a4dba835.png)
![image](https://user-images.githubusercontent.com/89113627/146694109-9f5b3146-a5ab-48f5-a5d6-8a19a9673d3f.png)

# SUMMARY

In determining which model is best at predicting high-risk loans, all the models were undersampled, oversampled, and also combined. Ensemble classifiers was evaluated where the dataset was resampled using BalancedRandomForestClassifier and EasyEnsembleClassifier models in order to predict which loans are high or low risk. Oversampling, undersampling, and mixed models have low recall and the accuracy score is not as high as Ensemble classifiers.

# RECOMMENDATION

Considering the best result amongst all the models evaluated, EasyEnsembleClassifier had the best balance of all the models because of its high accuracy score and a good balance of precision and recall scores. Therefore, I would recommend using EasyEnsembleClassifier to predict credit risk.

