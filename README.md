# Credit Risk Analysis
## Overview
### Purpose 
The purpose of this analysis was to build and assess machine learning models, which would be used to evaluate individual customer credit risk. The dataset used to train the models was from LendingClub. I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. I then evaluated the performance of these models to make a recommendation on which one should be used to predict credit risk. 
## Results
### Findings
In examining the results, I have paid close attention to the Balanced Accuracy Score as well as the Imbalanced Classification Report (ICR) from each model. Of particular importance in the ICR are two figures from the "f1" (F-score) column - the number from the bottom "avg / total" row, as well as the f-score from the "high risk" row. These rows display an ability to detect high credit risk individuals.
* Naive Random Oversampling 
![naive](https://user-images.githubusercontent.com/106560739/194462551-756ffc1b-29e6-4bc4-a376-f86d73285a2a.png)
This gave a balanced accuracy score of .64. The precision is low for high-risk loans and high for low-risk loans. The racall for high risk was .62 while the recall for low-risk was .65.
* SMOTE Oversampling
![Smote](https://user-images.githubusercontent.com/106560739/194462569-747c503c-0ae0-44cc-a9d4-35dd76d98b4b.png)
This gave a balanced accuracy score of .63. The precision was low for high-risk loans and high for low-risk loans. The recall for high-risk was .62 while the recall for low-risk was .64.
* Undersampling
![undersampling](https://user-images.githubusercontent.com/106560739/194462582-48ae8931-c0bd-4d32-9001-67c9de30df49.png)
This gave a balanced accuracy score of .50. The precision was low for high-risk loans and high for low-risk loans. The recall for high-risk was .59 while the recall for low-risk was .43.
* Combination Under-Over Sampling
![combination](https://user-images.githubusercontent.com/106560739/194462597-1c2bf99e-3141-4121-9e65-0d764c98020a.png)
This gave a balanced accuracy score of .63. The precision was low for high-risk loans and high for low-risk loans. The recall for high-risk was .70 while the recall for low-risk was .57.
* Balanced Random Forest Classifier
![balanced random](https://user-images.githubusercontent.com/106560739/194462609-d69c948f-3dfc-4430-93c1-a6767cd70a78.png)
This gave a balanced accuracy score of .78. The precision was low for high-risk loans and high for low-risk loans. The recall for high-risk was .67 while the recall for low-risk was .91.
* Easy Ensemble AdaBoost Classifier
![easy ensemble](https://user-images.githubusercontent.com/106560739/194462623-311d952e-738a-4de5-a43c-01fa2bd17737.png)
This gave a balanced accuracy score of .93. The precision was low for high-risk loans and high for low-risk loans. The recall for high-risk was .91 while the recall for low-risk was .94.
## Summary
### Conclusions
The highest compared balanced accuracy that is closest to 1 is the best machine learning model. For this project, the Easy Ensemble AdaBoost Classifier is the best model to choose since it is the highest with a balanced accuracy score of .93. The precision for all models were similar and within an appropriate range. The recall score also needs to fall within 0 and 1, with numbers closer to 1 being the better model. The Easy Ensemble AdaBoost Classifier had the highest recall score, making it again the best machine learning model to choose for further credit card analysis.
