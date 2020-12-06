# Analyzing Customer Churn using PySpark

## Project Overview

Online Services need to understand how customers are using and feeling about the product. As a data scientist one has to understand if the customers will continue to use the product with same enthusiam, will downgrade a paid service to free or will stop using the service. This is called customer churn.

Predicting churn rates is a challenging and common problem that data scientists and analysts regularly encounter in any customer-facing business.

In this project, we will be looking at Sparkify, a fictional music service provider similar to Spotify which needs a model to help predict customer churn. The data set consists of customer events with timestamps and is provided by udacity.

## Problem Statement and motivation

The dataset from Udacity for this research which included user logs for the past few months containing all the user activity. A user can have more than one sample as they can take multiple actions. The log contains some basic information about the user as well as information about a single action.

A user churn can be identified whenever there is an action for account cancellation page events for this product. This project is a part of the Udacity's Data Scientist Nanodegree program analyzing the behaviour of users for an app called Sparkify to predict user churn. 

As part of this project we will be creating a model using machine learning and the provided dataset and use that model to predict if a given user may leave or not. The model aims to predict which users are likely to cancel their account and based on that we will in future be able to take actions like provide discounts or offers to retain such users.

## Metrics

In this project we are trying to solve a classification problem of if a customer will churn or not and Accuracy will be used as metric for evaluating the model performance while trying to solve this problem.


## Files Description
Sparkify.ipynb is the main notebook where we do all the preprocessing, feature engineering and modelling. 
The dataset contains 18 columns and 286500 rows, the log file stored in JSON format. Each row represents user interactions with the service and information of the user’s session. Below is the schema for the data set.
root
 |-- artist: string (nullable = true)
 |-- auth: string (nullable = true)
 |-- firstName: string (nullable = true)
 |-- gender: string (nullable = true)
 |-- itemInSession: long (nullable = true)
 |-- lastName: string (nullable = true)
 |-- length: double (nullable = true)
 |-- level: string (nullable = true)
 |-- location: string (nullable = true)
 |-- method: string (nullable = true)
 |-- page: string (nullable = true)
 |-- registration: long (nullable = true)
 |-- sessionId: long (nullable = true)
 |-- song: string (nullable = true)
 |-- status: long (nullable = true)
 |-- ts: long (nullable = true)
 |-- userAgent: string (nullable = true)
 |-- userId: string (nullable = true)
 
## Data Pre-processing

We check for invalid,duplicate or missing data; for example, records without userids and sessionids. Convert categorical variables into numerical ones.

## Exploratory data analysis
We defined the variable churn and after that we do some exploratory analysis in order to find good predictors.

##

## Results 
I applied data processing to the small dataset and then extracted features that I thought would help predict the churn of the users. For this I used 4 Machine learning algorithms of LR, Random Forest, SVM and Gradient Boosted trees and saw that Random Forest Classifier did a better job at predicting the model. An attempt to further perform hyperparameter tuning to enhance the performance of the classifier did not provide any further gains in the classifier performance in making the prediction.

## Conclusion
I applied data processing to the small dataset and then extracted features that I thought would help predict the churn of the users. For this I used 4 Machine learning algorithms of LR, Random Forest, SVM and Gradient Boosted trees and saw that Random forest did a better job at predicting the model. An attempt to further perform hyperparameter tuning to enhance the performance of the classifier did not provide any further gains in the classifier performance in making the prediction.
It may be possible to try and add more features or choose any other classifier or try different hyperparameters setting to even try and improve the accuracy of the prediction via those trials as seen in the above Random Forest Classifier hyperparameters tuning.



## Tools & Software
* PySpark
* Spark MlLib
* Pandas
* Matplotlib
* Seaborn

## References
[Medium Blog post](https://capricioussunny.medium.com/analyzing-customer-churn-using-pyspark-abd6a558780f)
