# Credit_Risk_Analysis

## Overview 
In this project I used machine learning to analyze a credit card dataset and create six models that predict customer credit risk. I used several machine learning models and algorithms in an attempt to reduce bias and improve performance. In the results I will discuss the results of each model used and recommend which model should be used to predict credit risk.
 
## Results 
### Measures
Balanced Accuracy Score:
The accuracy score of a model is based on the difference between the predicted values and actual values. 

Precision Score: 
The precision score, also known as the positive predictive value, measures how likely a positive prediction is actually true. In other words, it is a measure of how reliable a positive classification is. Precision = TP/(TP+FP)

Recall Score:
A recall score, also referred to as sensitivity, is a measure of how likely all positive values will be predicted in a model. Sensitivity = TP/(TP+FN)

### Models
#### Model 1: Oversampling
Balanced accuracy score is .64
Precision: .01
Sensitivity: .74

#### Model 2: SMOTE Oversampling
Balanced accuracy score is .65 
Precision: .01
Sensitivity: .61

#### Model 3: Undersampling
Balanced accuracy score is .54
Precision: .01
Sensitivity: .67

#### Model 4: Combinaion (Over and Under) Sampling
Balanced accuracy score is .64
Precision: .01
Sensitivity: .72

#### Model 5: Ensemble Learner - Balanced Random Forest Classifier
Balanced accuracy score is .79
Precision: .03
Sensitivity: .70

#### Model 6: Ensemble Learner - Easy Ensemble AdaBoost Classifier
Balanced accuracy score is .93
Precision: .09
Sensitivity: .92

## Summary
In a model that predicts credit risk, the sensitivity score is more important. We are more concerned in capturing all of the true positive values rather than making sure all of the positive predictions are true.

### Recommendation
I would recommmend we use the Ensemble Learner - Easy Ensemble AdaBoost Classifier Model. When we look at the confusion matrix of this model we see that there are 101 values that are actually positive, only 8 of these were not predicted to be positive by the model. Compared to the other models tested, this model has the highest sensitivity score. 
