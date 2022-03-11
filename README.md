# Cardiovascular-Risk-Prediction
Cardiovascular disease(CVD) is the leading cause of death worldwide and a major public health concern. The most common type is coronary heart disease, which can cause a heart attack. Day by day the cases of Cardiovascular diseases(CVD) are increasing at a rapid rate and it's very important and concerning to predict any such diseases beforehand. In this study, we have provided a prediction model for 10-year risk assessment of Coronary Heart Disease(CHD) to predict whether the patient is likely to be diagnosed with a disease.

## Problem Statement
The aim of this project is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). Providing a valid model for cardiovascular disease risk classification of each population has become a high priority for scientists and organizations working in this field.

## Data Overview
For the project, the dataset we used is from cardiovascular study on residents of the town of Framingham, Massachusetts. It includes over 4,000 records and 15 attributes.
Each attribute is a potential risk factor. There are demographic, behavioral and medical risk factors.

## Methodology
![Screenshot (133)](https://user-images.githubusercontent.com/82964400/151691046-bbed0634-1f32-4f20-b469-d26bf938e0f9.png)

Our project consists of four phases namely- Data exploration, Data analysis, Data preparation and building models and analyzing their performance using various evaluation metrics.

For modeling we tried various regression models such as-

1)Logistic Regression

2)K-Nearest Neighbors

3)Support Vector Classifier

4)Decision Tree Classifier

5)Random Forest Classifier

6)Gradient Boosting Classifier

All these models were fine tuned using a grid search and randomized search method with repeated cross-validation (cv) to ﬁnd the best hyperparameters. We have also plotted variable importance plots for tree based models to determine the features that were most important while model building.

## Results

![results](https://user-images.githubusercontent.com/82964400/157888083-06b36b52-7e72-4d31-89b5-a0b6da011984.png)

After training the models with their best hyperparameters, the performance of each of the classification models were evaluated using the testing set with evaluation metrics. The model which provides the highest Accuracy is the best one.

![roc curve](https://user-images.githubusercontent.com/82964400/157888130-06193347-3ee3-42ba-a274-502877a347cd.png)

It is evident from the plot that the AUC for GradientBoosting classifier ROC curve is higher than that for the other models. Therefore, we can say that the Gradient Boosting classifier did a better job of classifying the positive class in the dataset.

## Conclusion

* Patients having higher sysBP and DiaBP tends to have high risk of Coronary heart disease
* The peoples of age above 55 have high risk of contracting disease and the risk increases with age
* Age, systolic BP and total cholesterol are the most influential features
* Gradient Boosting model is found to be the best model
* Therefore, Gradient Boosting model can be used to predict whether the patient will contract Coronary Heart Disease in next 10-years

