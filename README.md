# Analyzing Customer Churn using PySpark
## Project Overview
Predicting churn rates is a challenging and common problem that data scientists and analysts regularly encounter in any customer-facing business.
In this project, we will be looking at Sparkify, a fictional music service provider similar to Spotify which needs a model to help predict customer churn.

## Problem Definition and motivation
I got the dataset from Udacity for this research which included user logs for the past few months containing all the user activity. A user can have more than one sample as they could have taken multiple actions. A user churn can be identified whenever there is an action for account cancellation page events.
This project is a part of the Udacity's Data Scientist Nanodegree program analyzing the behaviour of users for an app called Sparkify to predict user churn.

## Files Description
Sparkify.ipynb is the main notebook where we do all the preprocessing, feature engineering and modelling. 

## Results 
I applied data processing to the small dataset and then extracted features that I thought would help predict the churn of the users. For this I used 3 Machine learning algorithms of Random Forest, SVM and Gradient Boosted trees and saw that Random Forest Classifier did a better job at predicting the model. An attempt to further perform hyperparameter tuning to enhance the performance of the classifier did not provide any further gains in the classifier performance in making the prediction.


## Tools & Software
* PySpark
* Spark MlLib
* Pandas
* Matplotlib
* Seaborn

## References
[Medium Blog post](https://capricioussunny.medium.com/analyzing-customer-churn-using-pyspark-abd6a558780f)
