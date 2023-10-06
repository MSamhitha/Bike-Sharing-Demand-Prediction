# Bike-Sharing-Demand-Prediction

## Project Overview

This project focuses on predicting bike-sharing demand using historical data. Bike-sharing systems are widely used for daily commuting and urban transportation. Accurate demand prediction helps in better resource allocation, which can lead to cost savings and improved customer satisfaction.

In this project, we leverage machine learning models to predict the number of bikes that will be rented at a specific hour based on various environmental and seasonal factors.

## Problem Statement

The main objective of this project is to build a predictive model that can accurately forecast bike rental demand. Given various features such as date, time, temperature, humidity, and more, the model should predict the number of bikes that will be rented in the future.

## Data Description

The dataset used in this project contains historical information related to bike rentals. Below are the details of the dataset columns:

- `Date`: The date of the rental record.
- `Hour`: The hour of the day (0-23).
- `Temperature(°C)`: The temperature in Celsius at the time of the rental.
- `Humidity(%)`: The humidity level at the time of the rental.
- `Wind Speed (m/s)`: The wind speed in meters per second.
- `Visibility (10m)`: The visibility in meters.
- `Solar Radiation (MJ/m2)`: The solar radiation in megajoules per square meter.
- `Rainfall(mm)`: The amount of rainfall in millimeters.
- `Snowfall (cm)`: The amount of snowfall in centimeters.
- `Seasons`: The season at the time of the rental (Spring, Summer, Autumn, Winter).
- `Holiday`: Indicates whether it was a holiday (Yes/No).
- `Functional Day`: Indicates whether it was a functional day (Yes/No).
- `Rented Bike Count`: The number of bikes rented during that hour.

The target variable for prediction in this project is `Rented Bike Count`, which represents the number of bikes rented during a specific hour.

Please note that data preprocessing, feature engineering, and outlier handling were performed to prepare the dataset for machine learning modeling.

## Evaluation Metrics

To evaluate the performance of our machine learning models, we use the following metrics:

- **Mean Squared Error (MSE)**: Measures the average squared difference between predicted and actual values.
- **Root Mean Squared Error (RMSE)**: The square root of MSE, providing a measure of the error in the same units as the target variable.
- **R-squared (R2) Score**: Represents the proportion of variance in the target variable that is predictable from the features. A higher R2 score indicates better model performance.

## Machine Learning Models

We have implemented and evaluated the following machine learning models:

1. Linear Regression
2. Ridge Regression
3. Lasso Regression
4. Random Forest Regressor

Hyperparameter tuning and cross-validation were applied to enhance model performance.

## Model Selection

The Random Forest Regressor model with hyperparameter tuning achieved the best performance, as evidenced by lower MSE and RMSE values and a higher R2 score.

## Feature Importance

Based on the Random Forest (CV) model, the most important features for predicting bike rental demand are temperature, hour of the day, functional day, and visibility.

## Conclusion

This project successfully developed a predictive model for bike sharing demand. Accurate demand forecasting can help in resource optimization and improve user experience. The Random Forest Regressor model demonstrated the best performance, and the key factors affecting bike rental demand were identified.

For detailed implementation and code, please refer to the project files.

