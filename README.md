# House Price Prediction

## Overview
The goal of this project is to predict the median house value using various regression models. The project involves data exploration, preprocessing, feature engineering, and model evaluation.

## Dataset
- [The dataset](https://www.kaggle.com/datasets/camnugent/california-housing-prices)

The dataset used in this project is the California housing dataset, which includes features like median income, house age, total rooms, total bedrooms, population, households, and proximity to the ocean.

## Exploratory Data Analysis
We started by exploring the dataset to understand the distribution of features and their correlation with the target variable.

## Preprocessing
Missing values:
- As they were few number of rows, we dropped them.
Scaling:
- We found some right-skewed features, So we applied logarithmic transformation to them.
Encoding:
- We found some non numerical features, So we encoded them.

## Feature Engineering
We Created new features:
- bedroom_ratio: Ratio of bedrooms to total rooms.
- household_rooms: Number of rooms per household.

## Modeling
We trained several regression models to see which one will give us the best performance on our data. They are:
- Random Forest Regressor
- XGBoost Regressor
- AdaBoost Regressor

## Hyperparameter Tuning
Performed hyperparameter tuning on the XGBoost model as it gave me the best performance. We using GridSearchCV to find the best parameters.

## Model Evaluation
Evaluated the models using metrics like R2 score, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).

## Conclusion
The project demonstrates the effectiveness of different regression models in predicting house prices, with XGBoost providing the best performance. Feature engineering and hyperparameter tuning significantly improved the model's accuracy.