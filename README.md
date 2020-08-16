# Cardiac_Arrhythmia_Detection_Classification
## Classification model building 

This database contains 279 attributes, 206 of which are linear valued, and the rest are nominal. The aim is to distinguish between the presence and absence of cardiac arrhythmia and to classify it in one of the 16 groups. Class 01 refers to 'normal' ECG classes 02 to 15 refers to different classes of arrhythmia, and class 16 refers to the rest of unclassified ones.

 ## Software and Libraries Used
- Language: Python 
- Software: Jupyter Notebook
- Libraries: Pandas, Numpy, Matplotlib, Sklearn, Seaborn


The following stages were performed 
1) Data Cleaning
2) Exploratory Analysis
3) Model Building
4) Prediction 

## 1) Data Cleaning
- Missing values are identified in columns J, T, QRST, P, heartrate in train dataset and T, P columns in Test dataset.
- Missing values in T, QRST, P and heartrate are replaced with mean or median based on the skewness of the distribution. whereas J has more than 90% missing values, so the column J is removed.

## 2) Exploratory Analysis
- Basic scatter plot is performed on 'age', 'sex', 'height', 'weight' parameters.

## 3) Model Building
After splitting the train data set in to train and validation datasets the following models are built on train dataset:
## Basic Models with grid search and Cross-validation

1. KNN Classification 
2. Logistic Regression
3. Random Forest
### PCA Models
4. KNN Classification 
2. Logistic Regression
3. Linear SVM 
4. Kernalised SVM 
5. Decision Trees
6. Random Forest

Compared PCA and Basic models for better prediction

7. Adaptive Boosting technique on Logistic regression

The Precision_macro function is used to evaluate the models. Logistic Regression has turned out to be a better performing model

## Prediction
Based on the logistic model the test data classes for Cardiac_Arrhythmia are predicted


 
        
