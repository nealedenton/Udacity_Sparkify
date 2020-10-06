# Udacity_Sparkify
Udacity Data Science Nanodegree capstone project


## Problem Statement

The aim of the project is to build a machine learning model to predict whether customer's of 'Sparkify' will 'churn' - i.e. they will cancel their account.
Sparkify is an imagined music streamling platform, similar to Spotify.  The raw data consists of web hits to the sparkify platform, including things like page name, timestamp and userId.

The dataset has been provided by Udacity for use in the captstone project of their Data Science Nanodegree.  The full datasetis very large and would require powerful server hardware to run the EDA and model building.  For the purposes of this project a small sample data set has been used to make it possible to run it on lower spec hardware.  However, the aim is to use a methodology that could scale to a large dataset, so a key principle has been to rely on PySpark rather than pandas and sckikit learn.

There is an accompanying blog post which discusses the project on medium here: https://medium.com/@nealedenton_87598/predicting-customer-churn-ee3b3a0bb370 

## Files Required
* Sparkify.ipynb : The notebook with the analysis
* README.md: This file
* mini_sparkify_event_data.json : (NOT INCLUDED) this can be obtained from Udacity if you enroll on the program


## Dependencies
* Apache Spark 2.4.3
* Jupyter Notebook environment

Python Packages
* pyspark.sql 
* pyspark.ml
* sklearn.metrics
* pandas
* numpy
* matplotlib.pyplot
* seaborn
* datetime

## Analysis

1. Import the necessary lirbaries
2. Import sample data set
3. Perform some initial Exploratory Data Analysis including:
    1. Identifying the 'label' we want our model to predict ('Cancellation Confirmation')
    2. Cleaning the data - removing rows with missing userId
4. Feature engineering: aggregate by userId and create relevant features
5. Modelling
    1. Split data into training and test set
    2. Logistic Regression with grid search to fine tune parameters with Cross Folds Validation
    3. Decision Tree Classification with grid search to fine tune parameters with Cross Folds Validation
6. Evaluation and Conclusion

