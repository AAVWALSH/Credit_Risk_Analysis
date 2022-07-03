# Credit_Risk_Analysis

### Overview
THe purpose of this practice was to employ different techniques to train and evaluate models with unbalanced classes to find the best to use on drastically imbalanced classes. Credit risk is inherently unbalanced as good loans outnumber risky loans. If a model predicted a majority of loans to be good that would technically be accurate when looking at overall numbers but but lacking the precision that would identify bad loans.
### Results
#### Naive Random Oversampling
Confusion Matrix:
[   57,    30],
[ 5734, 11384]

Accuracy Score: 0.6601016876770167

![image](https://user-images.githubusercontent.com/100727593/177055689-d5b4073b-abd6-4f79-88b3-eb4496d1c72e.png)

#### SMOTE Oversampling
Confusion Matrix:
[   55,    32],
[ 5812, 11306]

Accuracy Score:0.6463291312633204

![image](https://user-images.githubusercontent.com/100727593/177055676-e83928f1-dd22-4eae-a336-57de1578f0a1.png)

#### Undersampling
Confusion Matrix: 
[  51,   36],
[9684, 7434]

Accuracy Score:0.6463291312633204

![image](https://user-images.githubusercontent.com/100727593/177055666-a2cad94a-836c-42b7-a5c4-041c48493b71.png)

#### Combination/ SMOTEENN Sampling
Confusion Matrix:
[  61,   26],
[7294, 9824]
       
Accuracy Score: 0.5102433010624026

![image](https://user-images.githubusercontent.com/100727593/177055651-c10378ea-7be8-4e28-bd60-3287b70f0124.png)

#### Balanced Random Forest Classifer
Confusion Matrix:
[   58,    29],
[ 1560, 15558]

Accuracy Score: 0.9076431269979657

![image](https://user-images.githubusercontent.com/100727593/177055631-f1ef27b4-8f93-4bf9-a745-9d8571e8a6e1.png)

#### Easy Ensemble AdaBoost Classifier
Confusion Matrix
[   78,     9],
[  975, 16143]

Accuracy Score: 0.9428073234524847

![image](https://user-images.githubusercontent.com/100727593/177055621-cb8dedc5-4657-4223-9fe0-7f9344af0235.png)

### Summary

The Easy Ensemble AdaBoost Classfier had, by-far, the highest accuracy score out of all the models. This is because adaptive boosting is trained off a series of models and evaluates the errors of the preceding models. Each subsequent model gives extra weight to the errors from the previous to minimize erros in subsequent models. The process is repeated until the error rate is minimized. 
