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

Data Split:

<img   src="https://github.com/patelnehap/Credit_Risk_Analysis/blob/main/Images/Data_Split.JPG"  alt="Data Split"  title="Data Split" style="display: inline-block; margin: 0 auto; max-width: 300px">

### Naive Random Sampling:

<img   src="https://github.com/patelnehap/Credit_Risk_Analysis/blob/main/Images/Naive%20Rndm%20Sampling.JPG"  alt="Naive Random Sampling"  title="Naive Random Sampling" style="display: inline-block; margin: 0 auto; max-width: 300px">

1. Balanced Accuracy: 0.66
2. Precision: The precision is low for High-risk loans and is very good for Low-risk loans.
3. Recall: High/Low risk = .72/.60
4. F1 score : High/Low risk = .02/.75 (Low F1 score suggests a high number of False Positives in this model. Data needs to be resampled using Oversampling model to create a better model for accuracy.)

### SMOTE Oversampling

<img   src="https://github.com/patelnehap/Credit_Risk_Analysis/blob/main/Images/SMOTE.JPG"  alt="SMOTE"  title="SMOTE" style="display: inline-block; margin: 0 auto; max-width: 300px">

1. Balanced Accuracy: 0.66
2. Precision: The precision is low for High-risk loans and is very good for Low-risk loans.
3. Recall: High/Low risk = .62/.69
4. F1 score : High/Low risk = .02/.82(Low F1 score suggests a high number of False Positives in this model. Data needs to be resampled using Oversampling model to create a better model for accuracy.)

### SMOTEEN

<img   src="https://github.com/patelnehap/Credit_Risk_Analysis/blob/main/Images/SMOTEEN.JPG"  alt="SMOTEEN"  title="SMOTEEN" style="display: inline-block; margin: 0 auto; max-width: 300px">

1. Balanced Accuracy: 0.64
2. Precision: The precision is low for High-risk loans and is very good for Low-risk loans.
3. Recall: High/Low risk = .72/.54
4. F1 score : High/Low risk = .02/.72 (Low F1 score suggests a high number of False Positives in this model. Data needs to be resampled using Oversampling model to create a better model for accuracy.)

### Random Forest Sampler

<img   src="https://github.com/patelnehap/Credit_Risk_Analysis/blob/main/Images/RndmFrst.JPG"  alt="Random Forest Sampler"  title="Random Forest Sampler" style="display: inline-block; margin: 0 auto; max-width: 300px">

1. Balanced Accuracy: 0.67
2. Precision: The precision is low for High-risk loans and is very good for Low-risk loans.(Precision of 1 indicates that this model will not produce any false positives.)
3. Recall: High/Low risk = .35/1.0
4. F1 score : High/Low risk = .50/1.00 (F1 score of 1 suggests that this is a very good model to predict credit risk accuracy).


### Easy Ensemble

<img   src="https://github.com/patelnehap/Credit_Risk_Analysis/blob/main/Images/EasyEnsemble.JPG"  alt="Easy Ensemble"  title="Easy Ensemble" style="display: inline-block; margin: 0 auto; max-width: 300px">

1. Balanced Accuracy: 0.92
2. Precision: The precision is low for High-risk loans and is perfect 1 for Low-risk loans.
3. Recall: High/Low risk = .89/.94
4. F1 score : High/Low risk = .16/.97

## Summary

In conclusion, credit-risk is a difficult thing to predict, even for advanced machine learning algorithms. 
While the Random Forest Sampler model had the highest overall accuracy, this was largely due to the fact that the dataset was so radically unbalanced. 
Even when it's balanced accuracy was at 67%, it's F-score for high-risk prediction was no better than 0.50. Typically in machine learning models you want a good balance of recall and precision which is why I recommend the random forest sampler model over the other four models. It appears that the random forest model sampler had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.

