# Credit_Risk_Analysis

## Overview of the analysis

For this project we worked with a credit card dataset from LendingClub, a peer-to-peer lending services company, and we performed different machine learning models to make a recommendation on what model is the most convinient to perform a credit risk prediction.

## Results

### Logistic Regression Models


- Naive Random Oversampling

First we ran the Naive Random Oversampling model in which we obtained an average score of 0.99 in precision and 0.68 in recall. As for the high risk credits scores, we obtained 0.01 in precision and 0.63 in recall. On the other hand, in the low risk credits scores we obtained 1.00 in precision and 0.68 in recall. The model obtained a **balanced accuracy score** of **0.6526081124403125**. 


![naive-random](https://user-images.githubusercontent.com/107893200/201832226-b3e9b639-c2d7-4f03-bc31-3608953ba4a8.png)

- SMOTE Oversampling

As for the SMOTE model, we obtained an average score of 0.99 in precision and 0.68 in recall. The high risk credits scores were 0.01 in precision and 0.61 in recall. On the other hand, in the low risk credits scores we obtained 1.00 in precision and 0.68 in recall. The model obtained a **balanced accuracy score** of **0.6437309126495352**.


![SMOTE](https://user-images.githubusercontent.com/107893200/201832314-4cd83626-4e07-4c94-8b8b-3517a108a411.png)


- Cluster Centroids

As for the Cluster Centroids model, we obtained an average score of 0.99 in precision and 0.44 in recall. The high risk credits scores were 0.01 in precision and 0.57 in recall. On the other hand, in the low risk credits scores we obtained 0.99 in precision and 0.43 in recall. The model obtained a **balanced accuracy score** of **0.5009765130679805**. 


![cluster-centroids](https://user-images.githubusercontent.com/107893200/201832418-6eb4fba0-7760-4831-b8be-54a8562721ff.png)


- SMOTEENN

As for the SMOTEENN model, we obtained an average score of 0.99 in precision and 0.56 in recall. The high risk credits scores were 0.01 in precision and 0.75 in recall. On the other hand, in the low risk credits scores we obtained 1.00 in precision and 0.56 in recall. The model obtained a **balanced accuracy score** of **0.6565668921997064**.

![SMOTEENN](https://user-images.githubusercontent.com/107893200/201832486-a18c2ae4-4939-436d-9745-65036f1c0b68.png)


### Ensemble Models
As for the ensemble models of machine learning we got the next results:

- Balanced Random Forest Classifier

In the Balanced Random Forest Classifier model we got an average precision of 0.99 and a recall of 0.90. Specifically in high risk credits we obtained 0.04 precision and 0.72 recall, these being very low numbers. In low risk credits we obtained 1.00 precision and 0.90 recall. In the general overview of the model, it obtained a **balanced accuracy score** of **0.8107896709563742**.

![random-forest](https://user-images.githubusercontent.com/107893200/201830805-ba13cdc5-1aab-462d-83b3-604c9d6c8579.png)

- Easy Ensemble AdaBoost Classifier

As for the AdaBoost machine learning model, we obtained a total of 0.99 precision and 0.95 recall. For high risk credits we obtained a 0.09 precision score and 0.93 recall score, while for low risk credits we obtained 1.00 precision score and 0.95 recall score. The model obtained a **balanced accuracy score** of **0.9368833896965066**. 


![adaBoost](https://user-images.githubusercontent.com/107893200/201830908-3dc65554-d4fe-40c5-9237-69ed4a5ea5be.png)


## Summary

After testing different machine learning models and observing the precision, recall and balanced accuracy scores of each one, we can conclude the following. 

The models that obtained a better balanced accuracy score were the SMOTEENN with a 0.65 score, the Balanced Random Forest Classifier with a 0.81 score, and the AdaBoost Classifier with a 0.93 score. The latter obtained the best among all the other models.

The machine learning model we recommend as the most suitable for performing a credit risk prediction is the Easy Ensemble AdaBoost Classifier. 
This is due to the fact that in both the precision and recall scores for high risk loans we obtained a better percentage, although it still has a low score of 0.09 in precision and 0.93 for recall. In this particular case we are interested in obtaining a high recall score. This is because we want the model to detect the least amount of false positives but to correctly detect who is a high risk when authorizing a credit. 
