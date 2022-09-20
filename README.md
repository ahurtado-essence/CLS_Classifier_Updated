# CLS_Classifier_Updated

Building a classification model to predict whether a study is significant or not.

The models used are Logistic Regression, SVM, Naive Bayes, KNN, XGBoost and Random Forest. Categorical variables in the dataset were transformed into dummy variables, and numerical features were scaled using scikit learn's RobustScaler. 

Two methods were used to evaluate the models:

1. Normal K-fold cross validation was used with gridsearch to find the best performing models for each of the following metrics: accuracy, AUC and f1 score. 
2. Nested K-fold cross validation was used with gridsearch to find the highest accuracy model. This method improves upon the first in reducing the chance of overfitting on the data and increasing accuracy scores across all models. 
