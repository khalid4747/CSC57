# Real Estate Regression Model 
### CSC5800 ML Project

## Objective: 
### Build a regression model with machine learning to predict is $value/unit of area
Data set from https://archive.ics.uci.edu/ml/datasets/-Real+estate+valuation+data+set

6 different variables

`X1`=the transaction date

`X2`=the house age (unit: year)

`X3`=the distance to the nearest MRT station (unit: meter)

`X4`=the number of convenience stores in the living circle on foot (integer)

`X5`=the geographic coordinate, latitude. (unit: degree)

`X6`=the geographic coordinate, longitude. (unit: degree)

The output is normalized for the amount of square footage of the house. 
The output we’re predicting is **(10000 New Taiwan Dollar/Ping (also 3.3 meters))** which is similar to $/sq ft in America.
We want to predict what the “$/sq ft.” given the 6 features. 

#Results 
There was a total of four different algorithms used to try and predict the house’s value. Since we are trying to predict a numerical value, we must use regression model. The first algorithm is a simple linear regression model which preformed with an accuracy of 61%. This wasn’t amazing but it was the first step. The r^2 value was .53 and the mean squared error was 82.1. With 5-fold cross validation the result of the outcome did change significantly. The data then was split from 70% 30% to 80% 20% which did not help the accuracy.

Next was to test the different types of regression models that were available so I used simple vector regression model, linear Bayesian model, and K nearest neighbor.

The best one turned out to nearest neighbor with an accuracy of 67%. This algorithm outperformed all the other ones which relatively low residuals. There are still a few outliers but the general performance is satisfactory.
