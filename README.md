# Linear Regression Analysis for Auto MPG Dataset

**Authors:**  
Kunal Yadav (mailmekunal2002@gmail.com)

**Date:**  
September 11, 2023

## Introduction

This report explores the application of linear regression on the Auto MPG dataset. The dataset contains information about various car attributes like cylinders, displacement, horsepower, weight, acceleration, year of manufacture, and more, with the target variable being miles per gallon (mpg). The goal is to build a regression model to predict the mpg based on these attributes.

## Data Preprocessing

- The dataset was loaded and examined for any missing values.
- The 'car_name' column was dropped as it was not relevant to our analysis.
- The 'origin' column was converted to categorical values ('america', 'europe', 'asia') using one-hot encoding.
- Missing values in the 'hp' column were replaced with the median value.
- Data scaling was performed using z-score normalization.

## Exploratory Data Analysis

- Data distributions and relationships were visualized using pair plots.
- The correlation between variables was analyzed.

## Model Building

- Linear regression models were built to predict mpg.
- The dataset was split into training and testing sets.
- The following variables were used as predictors: 'cyl', 'disp', 'hp', 'wt', 'acc', 'yr', and 'car_type'.
- Coefficients and intercepts were calculated for the linear regression model.
- The R-squared values for both the training and testing sets were calculated.

## Model Evaluation

- Model performance was assessed using mean squared error (MSE).
- Residual plots were created to visualize the model's performance.
- Both standardized and non-standardized data were used to build and evaluate the model.

## Results

- The linear regression model achieved an R-squared value of 0.826 on the training set and 0.840 on the testing set, indicating a good fit.
- The model's MSE on the testing set was approximately 0.391.
- Residual plots showed that the model had a reasonable fit to the data.

## Conclusion

In this analysis, we successfully built and evaluated a linear regression model for predicting mpg based on various car attributes. The model performed well, with a high R-squared value and low MSE, suggesting that it can effectively predict the fuel efficiency of cars in the Auto MPG dataset. Further optimizations and feature engineering could potentially enhance the model's performance.
