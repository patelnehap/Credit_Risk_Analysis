# Credit_Risk_Analysis

## Overview: 
Credit risk is associated with the possibility of a client failing to meet contractual obligations, such as mortgages, credit card debts, and other types of loans.
Minimizing the risk of default is a major concern for financial institutions. For this reason, financial institutions are increasingly relying on technology to predict which clients are more prone to stop honoring their debts.
Machine Learning models have been helping these companies to improve the accuracy of their credit risk analysis, providing a scientific method to identify potential debtors in advance.
Being able to predict credit risk with machine learning algorithms can help banks and financial institutions predict anomalies, reduce risk cases, monitor portfolios, and provide recommendations on to reject fradulent applications.
To complete this analysis, we use different Machine Learning techniques to train and evaluate the data with unbalanced classes. 
The dataset from the LendingClub has an unbalanced classification problem due to the number of good loans outweighing the amount of risky loans. 
In order balance out the classifications to allow for more meaningful predictions and improve the accuracy score, we needed to employ various Machine Learning algorithms to resample the data. 
These algorithms include RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier.

## Results:
The results for the six machine learning models including their respective balanced accuracy, precision, and recall scores are as follows:

### Naive Random Sampling:

<img   src="https://github.com/patelnehap/Amazon_Vine_Analysis/blob/main/Images/GreaterThan20.JPG"  alt="Greater Than 20"  title="Greater than 20" style="display: inline-block; margin: 0 auto; max-width: 300px">

1. Balanced Accuracy: 0.6612700484668286
2. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
3. Recall: High/Low risk = .66/.67

### SMOTE Oversampling

<img   src="https://github.com/patelnehap/Amazon_Vine_Analysis/blob/main/Images/GreaterThan20.JPG"  alt="Greater Than 20"  title="Greater than 20" style="display: inline-block; margin: 0 auto; max-width: 300px">

1. Balanced Accuracy: 0.6303296388959394
2. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
3. Recall: High/Low risk = .62/.64

### SMOTEEN

<img   src="https://github.com/patelnehap/Amazon_Vine_Analysis/blob/main/Images/GreaterThan20.JPG"  alt="Greater Than 20"  title="Greater than 20" style="display: inline-block; margin: 0 auto; max-width: 300px">

1. Balanced Accuracy: 0.6303296388959394
2. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
3. Recall: High/Low risk = .62/.64

### Random Forest Sampler

<img   src="https://github.com/patelnehap/Amazon_Vine_Analysis/blob/main/Images/GreaterThan20.JPG"  alt="Greater Than 20"  title="Greater than 20" style="display: inline-block; margin: 0 auto; max-width: 300px">

1. Balanced Accuracy: 0.6303296388959394
2. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
3. Recall: High/Low risk = .62/.64

### Easy Ensemble

<img   src="https://github.com/patelnehap/Amazon_Vine_Analysis/blob/main/Images/GreaterThan20.JPG"  alt="Greater Than 20"  title="Greater than 20" style="display: inline-block; margin: 0 auto; max-width: 300px">

1. Balanced Accuracy: 0.6303296388959394
2. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
3. Recall: High/Low risk = .62/.64

## Summary

In conclusion, credit-risk is a difficult thing to predict, even for advanced machine learning algorithms. 
While the Easy Ensemble AdaBoost Classifier model had the highest overall accuracy, this was largely due to the fact that the dataset was so radically unbalanced. 
Even when it's balanced accuracy and average F-score were above 90%, it's F-score for high-risk prediction was no better than 0.16. Typically in machine learning models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.

