# Canada Major Cities House Price Prediction

## Overview
This project develops a machine learning model to predict house prices across major cities in Canada. The model leverages a dataset comprised of features like the number of bedrooms and bathrooms, city population, geographical coordinates, and the city name to predict the market value of homes.

## Data
The dataset encompasses property listings from major Canadian cities with the following features:
- `Number_Beds`: Number of bedrooms in the house.
- `Number_Baths`: Number of bathrooms in the house.
- `Population`: Population of the city where the house is located.
- `Latitude`: Geographical latitude of the house location.
- `Longitude`: Geographical longitude of the house location.
- `City`: Name of the city where the house is located.

## Preprocessing
Data preprocessing involves several steps:
- Categorical variable `City` is encoded numerically with `LabelEncoder`.
- Numerical features are scaled using `StandardScaler` to ensure data normalization.

## Modeling
Two predictive models were developed and evaluated:
- `LinearRegression`: Serves as a baseline model.
- `RandomForestRegressor`: An ensemble model optimized with `GridSearchCV` for hyperparameter tuning.

## Evaluation
Model performance is assessed using the Mean Squared Error (MSE) and R-squared metrics to gauge accuracy and fit.

## Prediction
For making predictions with the trained models, the following steps are executed:
1. Input features undergo the same preprocessing as the training data.
2. The model's `predict` method is then invoked to estimate house prices.

## Author
Vishal Thilak
