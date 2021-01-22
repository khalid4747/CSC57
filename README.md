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
