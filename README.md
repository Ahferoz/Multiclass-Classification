# Multiclass-Classification
Apply Multiclass Classification On Real World Problem

We have used Music Genre Data for Multiclass classification .Here you can learn how to apply multiclass classification. How to  improve performance of model using different techniques.Data was highly skewed so performance was very low.There are 


# Things you can learn from here.

## Exploratory Data Analysis(EDA)
- In EDA, we get the insights of our data as much as possible such data type of each variable , missing values, relationship among the variables,distribution of varibales etc.Most   of the time we get the data with missing values so imputing the missing values depends on how good you study the data.

- Target distribution in training and validation set. 
  
  We have similar distribution of each category in Training ,Validation set.

- Different Kinds of plots between targets and features using matplotlib and seaborn .

  It is good to use visualization libraries to understand the relationship between features and the target variables.We have used different types of plot to understand the         relationship between target and feature so that we can decide which feature is strongly related to target variable.

- Imputing missing values

  Handling with missing values is an important factor to have great impact on model performance.We have missing values in Popularity, Key and Instrumentalness features.We have     filled Popularity missing values with mean and Key , Instrumentalness features with median.

  

## Data preprocessing pipline.
  
  Basically it is user defined function that we use to fill missing values and transform categorical variables into numeric values.This function is uesd to fill training ,         validation and test set.
  
  We have only missing values in our data set and do not have any categorical variable to encode.
  
## Model Selection 
 
 Here we train different models on our training set to select the one which performe better then do the experiment with the selected one to enhance the model performance.
 
 We have train three model Logistic Regression ,Decision Classifier and Random Forest Classifier on training set to get the idea which is to be selected.We have found that Random Forest is performing better than others two.


## Experiments with Random Forest to enhance performance

  Doing experiments mean to drop less import features , use different imputing method or add new features using existing features so that model performance can be increased.
  
  Below are the experiments that we have done.
  
  Experiment 1: Remove samples of the class doing very bad in performance.
  
  we have noticed that class 1 and class 6 samples have high variance.
  
  Experiment 2: Oversampling for the class doing very bad in performance

  We done oversampling of class 1 and class 6  so that it can help model to get right pattern.

  Experiment 3 : Oversampling of overall data for week Classes
  
  we done oversampling of overall data before split.
   
  Experiment 4:Random Forest on Oversampled Data Using CV
  
  We have used cross-validation techniques to help model to get pattern for each class
    
  Experiment 5:Random Forest on Oversampled Data of class 2 and 8 Using CV
  
  We have done oversampling of class 2 and class 8 because of low score these classes.
   
 ## Final Model: Random Forest with CV=5
 
 we have got mean F1-macro scrore=0.76
