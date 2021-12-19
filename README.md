# Credit_Risk_Analysis
# Project Overview
This project focuses on how to apply machine learning to solve a real-world challenge: credit card risk.
Credit risk is considered to be an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, different techniques will be employed to train and evaluate models with unbalanced classes.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, one will oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm will be used. Next, one will compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Afterwards, the performance of these models will be evaluated and one will make a written recommendation on whether they should be used to predict credit risk.

# Deliverable 1: Use Resampling Models to Predict Credit Risk

Using the knowledge of the imbalanced-learn and scikit-learn libraries, one will evaluate three machine learning models by using resampling to determine which is better at predicting credit risk. First, one will use the oversampling RandomOverSampler and SMOTE algorithms, and then use the undersampling ClusterCentroids algorithm. Using these algorithms, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.
