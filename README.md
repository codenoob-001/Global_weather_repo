Overview

This project focuses on analyzing global climate data, identifying trends, and applying machine learning models for forecasting and anomaly detection.

Dataset

We use the GlobalWeatherRepository.csv dataset, which includes climate variables such as temperature, precipitation, humidity, and wind speed across multiple regions. Additional shapefiles are used for geographical analysis.

Methodology

1. Data Cleaning & Preprocessing

Handling Missing Values: Imputed missing temperature and precipitation values using mean/median imputation.

Data Type Conversion: Converted date columns to datetime format and ensured numerical columns were correctly formatted.

Removing Duplicates: Dropped duplicate rows to avoid redundancy.

Outlier Detection: Used Z-score and IQR methods to identify and handle anomalies in temperature and precipitation.

2. Exploratory Data Analysis (EDA)

Summary Statistics: Examined min, max, mean, and standard deviation of key weather variables.

Correlations: Heatmaps and scatter plots were generated to explore relationships between temperature, precipitation, humidity, and wind speed.

Trend Analysis: Used line plots to observe seasonal trends over time.


3. Forecasting Models

Implemented multiple machine learning models to predict future weather conditions:

Random Forest Regressor: Applied for temperature prediction using historical weather data.

XGBoost Regressor: A gradient boosting approach for improved accuracy.

Linear Regression: A baseline model to compare performance.

SARIMA: Time series forecasting model for trend-based predictions.

4. Model Evaluation

Each forecasting model was evaluated using:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

R-squared (R²) Score

These metrics helped assess model performance and select the best forecasting approach.

SARIMA performed the best followed by XG boost


