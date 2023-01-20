# Credit_Risk_Analysis

## Overview of the analysis: 
This is a machine learning project involving evaluating credit card risk. The challenge of credit risk is that there are often many more good loans than risky loans, making it an unbalanced classification problem. The goal of the of the project is to use resampling techniques and machine learning models to predict credit risk. Using the imbalanced-learn and scikit-learn libraries, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. I also used a combination of over- and undersampling using the SMOTEENN algorithm. Additionally, I compared two machine learning models that reduce bias, the BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results: 

### Naive Random Oversampling
In this case, class "1" has a precision of 1.00, meaning that all of the instances predicted as class "1" were actually class "1". Its recall is 0.62, meaning that it correctly predicted 62% of all actual class "1" instances. Its specificity is 0.64, meaning that it correctly predicted 64% of all actual class "0" instances. The f1-score for class "1" is 0.76, indicating a relatively high level of precision and recall.

On the other hand, class "0" has a much lower precision of 0.01, meaning that only 1% of the instances predicted as class "0" were actually class "0". Its recall is 0.64, meaning that it correctly predicted 64% of all actual class "0" instances. Its specificity is 0.62, meaning that it correctly predicted 62% of all actual class "1" instances. The f1-score for class "0" is 0.02, indicating a very low level of precision and recall.

The overall precision, recall, and f1-score for the classifier are 0.62, 0.62, and 0.76 respectively. The model is not performing well on either class, it is struggling in identifying class 0 and not able to correctly identify class 1. It is likely that the model needs to be retrained or improved to better handle imbalanced data.

![Test](/Resources/naive.png)

### SMOTE Oversampling
In this case, class "1" has a precision of 1.00, meaning that all of the instances predicted as class "1" were actually class "1". Its recall is 0.66, meaning that it correctly predicted 66% of all actual class "1" instances. Its specificity is 0.63, meaning that it correctly predicted 63% of all actual class "0" instances. The f1-score for class "1" is 0.80, indicating a relatively high level of precision and recall.

On the other hand, class "0" has a much lower precision of 0.01, meaning that only 1% of the instances predicted as class "0" were actually class "0". Its recall is 0.63, meaning that it correctly predicted 63% of all actual class "0" instances. Its specificity is 0.66, meaning that it correctly predicted 66% of all actual class "1" instances. The f1-score for class "0" is 0.02, indicating a very low level of precision and recall.

The overall precision, recall, and f1-score for the classifier are 0.66, 0.66, and 0.79 respectively. The model is not performing well on either class, it is struggling in identifying class 0 and not able to correctly identify class 1. It is likely that the model needs to be retrained or improved to better handle imbalanced data.

### ClusterCentroids Undersampling 
In this case, class "1" has a precision of 1.00, meaning that all of the instances predicted as class "1" were actually class "1". Its recall is 0.56, meaning that it correctly predicted 56% of all actual class "1" instances. Its specificity is 0.61, meaning that it correctly predicted 61% of all actual class "0" instances. The f1-score for class "1" is 0.72, indicating a relatively high level of precision but lower level of recall.

On the other hand, class "0" has a much lower precision of 0.01, meaning that only 1% of the instances predicted as class "0" were actually class "0". Its recall is 0.61, meaning that it correctly predicted 61% of all actual class "0" instances. Its specificity is 0.56, meaning that it correctly predicted 56% of all actual class "1" instances. The f1-score for class "0" is 0.01, indicating a very low level of precision and recall.

The overall precision, recall, and f1-score for the classifier are 0.56, 0.56, and 0.71 respectively. The model is not performing well on either class, it is struggling in identifying class 0 and not able to correctly identify class 1. It is likely that the model needs to be retrained or improved to better handle imbalanced data.

### Combination (Over and Under) Sampling
In this case, class "1" has a precision of 1.00, meaning that all of the instances predicted as class "1" were actually class "1". Its recall is 0.60, meaning that it correctly predicted 60% of all actual class "1" instances. Its specificity is 0.71, meaning that it correctly predicted 71% of all actual class "0" instances. The f1-score for class "1" is 0.75, indicating a relatively high level of precision but lower level of recall.

On the other hand, class "0" has a much lower precision of 0.01, meaning that only 1% of the instances predicted as class "0" were actually class "0". Its recall is 0.71, meaning that it correctly predicted 71% of all actual class "0" instances. Its specificity is 0.6, meaning that it correctly predicted 60% of all actual class "1" instances. The f1-score for class "0" is 0.02, indicating a very low level of precision and recall.

The overall precision, recall, and f1-score for the classifier in this case are 0.60, 0.60, and 0.74 respectively. In this case, the model is not performing well as it is struggling in identifying class 1 and not able to correctly identify class 0. It is likely that the model needs to be retrained or improved to better handle imbalanced data

### Balanced Random Forest Classifier
In this case, class "1" has a precision of 1.00, meaning that all of the instances predicted as class "1" were actually class "1". Its recall is 0.97, meaning that it correctly predicted 97% of all actual class "1" instances. Its specificity is 0.48, meaning that it correctly predicted 48% of all actual class "0" instances. The f1-score for class "1" is 0.99, indicating a high level of precision and recall.

On the other hand, class "0" has a much lower precision of 0.09, meaning that only 9% of the instances predicted as class "0" were actually class "0". Its recall is 0.48, meaning that it correctly predicted 48% of all actual class "0" instances. Its specificity is 0.97, meaning that it correctly predicted 97% of all actual class "1" instances. The f1-score for class "0" is 0.15, indicating a very low level of precision and recall.

The overall precision, recall, and f1-score for the classifier are 0.97, 0.97, and 0.98 respectively. The model is performing well on class 1, with a high precision and recall, but is struggling on class 0 where the precision is low, meaning that the model is not able to identify the class 0 correctly. It is likely that the model needs to be retrained or improved to better handle imbalanced data.

### Easy Ensemble AdaBoost Classifier
In this case, class "1" has a precision of 1.00, meaning that all of the instances predicted as class "1" were actually class "1". Its recall is 0.97, meaning that it correctly predicted 97% of all actual class "1" instances. Its specificity is 0.44, meaning that it correctly predicted 44% of all actual class "0" instances. The f1-score for class "1" is 0.99, indicating a high level of precision and recall.

On the other hand, class "0" has a much lower precision of 0.08, meaning that only 8% of the instances predicted as class "0" were actually class "0". Its recall is 0.44, meaning that it correctly predicted 44% of all actual class "0" instances. Its specificity is 0.97, meaning that it correctly predicted 97% of all actual class "1" instances. The f1-score for class "0" is 0.13, indicating a very low level of precision and recall.

The overall precision, recall, and f1-score for the classifier are 0.97, 0.97, and 0.98 respectively.The model is performing well on class 1, with a high precision and recall, but is struggling on class 0 where the precision is low, meaning that the model is not able to identify the class 0 correctly. It is likely that the model needs to be retrained or improved to better handle imbalanced data.

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
The EasyEnsembleClassifier model performed the best among the six models evaluated, with a 97% accuracy rate and a 8% precision rate when identifying "High Risk" candidates. It also had the highest sensitivity or recall rate at 97%  and an F1 score of 98%. Therefore, it is recommended for this type of analysis. The other models ranked in descending order based on "High Risk" results are: BalancedRandomForestClassifier, SMOTE, SMOTEENN, RandomOverSampler, and ClusterCentroids. It is important to note that the original dataset had 99% of the applications classified as "Low Risk" with only 1% of the data classified as "High Risk" which may skew the results and not be acceptable for banks.




