# Predicting User Churn with PySpark

## Overview 

In this project, one of the most common real-world problem is taken as a case: predicting churn rates. 
It is a challenging problem for many businesses to predict which users are at risk to churn.   
Accurate identification of these users before they leave is crucial for the business revenue. 
User specific incentives, discounts are potential savings for the businesses. 
You can use this repo to learn how to deal with big data using Spark and build useful model for predicting churn. 

Here a Machine Learning model is developed to predict user churn by user behavior events in a music streaming app.
The steps followed in the development:
#### 1. Data preprocessing
Loading and clean of the dataset. Invalid or missing data like records without userids or sessionids are handled. 
#### 2. Exploratory Data Analysis (EDA)
EDA is performed with Spark functionalities. 
#### 3. Feature Engineering
For the model label 'Churn' is defined from Cancellation Confirmation events which includes paid and free users. 
EDA is performed to observe user behaviour in churn and illustrated with plots.
Aggregates on these two groups of users, observing how much of a specific action they experienced per a certain 
time unit and number of songs played are explored.
#### 4.  Training of the Model and Parameter Tuning
The full dataset split into train, test, and validation sets. 
Logistic Regression, Random Forest Classifier, GBT Classifier, Linear SVC and Naive Bayes 
Machine learning methods are tested. The accuracy of the models are measured and reported.
The best model's parameters are further tuned. The winning model is evaluated based on test accuracy and 
report results on the validation set. For the optimization F1 score is selected as the metric due to the
size of the churned user subset. 

### Dataset 
User generates data upon interaction with the service: playing songs, logging out, liking a song, hearing an ad or downgrading their service.
This interaction creates a timestamp and contains key insights for keeping business thrive.

### Files
* mini_sparkify_event_data.json: JSON dataset.
* read_and_write_data_Spark.ipynb: Notebook for Spark functionalities.
* Sparkify_Data_Scientist_Capstone_Project.ipynb: Notebook for the model.

## Libraries and Modules 

* [pyspark.sql](https://spark.apache.org/docs/2.4.0/api/python/pyspark.sql.html)
* [pyspark.ml](http://spark.apache.org/docs/latest/ml-guide.html)
* [pandas](https://pandas.pydata.org/)
* [numpy](https://numpy.org/) 
* [seaborn](https://seaborn.pydata.org/#)

### Further Links
Medium Article Link: https://medium.com/@aysegulturupcu/predicting-user-churn-with-p-db4719880280
