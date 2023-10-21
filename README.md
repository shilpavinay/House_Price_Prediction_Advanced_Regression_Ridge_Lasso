# House_Price_Prediction_Advanced_Regression_Ridge_Lasso

## Problem Statement

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. 
For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below. 

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know: 

Which variables are significant in predicting the price of a house, 
How well those variables describe the price of a house.
Also, determine the optimal value of lambda for ridge and lasso regression.

## Business Goal 

You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. 
They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

## Conclusion :

### The company wants to know:

#### Which variables are significant in predicting the price of a house
Five Most Important Predictor Variables – I will be reviewing the coefficients of the Lasso regression model to determine which five predictor variables have the largest non-zero coefficients. These are the five most important variables in your initial model.

Below are the coefficient values from my analysis and the top 5 predictor variables are listed below.

MSZoning_RL GrLivArea MSZoning_RM OverallQual MSZoning_FV

Since Lasso helps in feature reduction (as the coefficient value of one of the feature became 0), Lasso has a better edge over Ridge.

Based on Lasso, the factors that generally affect the price are:

1. The Zoning classification,
2. Living area square feet,
3. Overall quality and condition of the house,
4. Foundation type of the house,
5. Number of cars that can be accomodated in the garage,
6. Total basement area in square feet and the Basement finished square feet area

Therefore, the variables predicted by Lasso in the above bar chart as significant variables for predicting the price of a house.

#### How well those variables describe the price of a house. Also, determine the optimal value of lambda for ridge and lasso regression.

The variables predicted by Lasso from our analysus are significant variables for predicting the price of a house.

1. The optimal lambda value of Ridge and Lasso is as specified below from the model analysis.
Ridge – 6
Lasso – 0.0004

2. The mean squared in case of Ridge and Lasso are from my analysis are.
Ridge – 0.013698622121799814
Lasso - 0.013481512842345686

Please note that, the mean squared value of Lasso lower than that of a Ridge.

As per learning below are the techniques.

##### Consider Ridge Regression when:
If there are many features, and multicollinearity (high correlation between features) is a concern. If we believe that most features are relevant and don't want them to be eliminated entirely and our
goal is to reduce overfitting while retaining all features.

##### Consider Lasso Regression when:
If there are many features, but they look like many of them are irrelevant or redundant. If I want to select a subset of the most important features and eliminate the rest and finally, if I prefer a more
interpretable and sparser model.

Lasso helps in feature reduction as the coefficient value of one of the features became 0. Therefore, the variables predicted by Lasso can be applied to choose significant variables for predicting the
price of the house. 
