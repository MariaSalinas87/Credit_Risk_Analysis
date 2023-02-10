# Credit_Risk_Analysis

1.	Overview of the analysis: Explain the purpose of this analysis.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I need to employ different techniques to train and evaluate models withunbalanced classes. Jill asked me  to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Then I  compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. At the end I evaluated the performance of these models and make a written recommendation on whether they should be used to predict credit risk.


2.	Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.


RandomOversampler
Balance Accuracy Score 66.29%

![image](https://user-images.githubusercontent.com/112505962/218166686-1a011ff1-53f9-4928-bf0c-db9e45c2e2f7.png)



Combination sampling using SMOTEEN

Balance Accuracy Score: 66.29

 
![image](https://user-images.githubusercontent.com/112505962/218166716-5055958b-117f-4be4-aa5e-9a1a4e76acd2.png)



Balanced RandomForestClassifier
Balance accuracy score= 78.78
 
![image](https://user-images.githubusercontent.com/112505962/218166749-bec05fba-7b8d-4811-a9d5-789316ea5082.png)



EasyEnsembleClassifer
Accuracy score- 92.5%

 
![image](https://user-images.githubusercontent.com/112505962/218166765-880d0860-2cf6-4005-b87a-82632cc1d663.png)


Confusion matrix
Accuracy score-64.39%
 
![image](https://user-images.githubusercontent.com/112505962/218166781-b157c620-03e6-4dfb-b8c5-90d6d4e81ae4.png)



3.	Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.


Based on the results, it seems likes the EasyEnsemble in AdaBoost is the best method. It had a 92.54% accuracy.  The balancing is achieved by random under-sampling. 
