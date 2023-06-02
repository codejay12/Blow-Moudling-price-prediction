# Blow Moulding Price Prediction

## Introduction
Predicting the price of blow moulding contracts can be valuable for various stakeholders, including manufacturers, suppliers, and customers. Accurate price predictions can assist manufacturers in determining optimal pricing strategies, negotiating contracts, and managing production costs. Suppliers can use price predictions to optimize their supply chain and inventory management, while customers can make informed decisions based on price forecasts when procuring blow moulding services.

## Dataset
The provided dataset consists of 276 rows and 50 columns, representing data on a monthly basis from the years 2000 to 2022. The dataset includes various columns with missing data and covers commodities, market prices, protests, and import/export information. It includes columns related to commodity prices, producer price indices, and export/import data for specific countries.

## Exploratory Data Analysis (EDA)
EDA revealed seasonality patterns in the time series, indicating recurring patterns or fluctuations within each year. An uptrend was observed until 2015, followed by a subsequent uptrend from 2016 onwards. Analysis of export and import data showed variations among countries, with the USA consistently exporting blow moulding goods. The correlation between blow moulding prices and oil prices changed after 2014, indicating a divergence between the two.

## Pre-processing
Pre-processing involved handling missing values and creating additional features. Columns with null percentages exceeding 80% were removed, and missing values in specific columns were imputed with appropriate values. Iterative imputation yielded satisfactory results for handling missing values. Additional features were created to capture temporal information, and lag features were generated to consider historical behavior and trends in the data.

## Model Building
Two approaches were used for model building:
1. Univariate Analysis: Smoothing techniques such as rolling mean, exponential smoothing, and Facebook Prophet were employed using the date and target variables.
2. Bivariate Analysis: Exogenous columns and lag columns were included, and models such as Auto-ARIMA, SARIMA, LSTM, Lazy Predict AUTOML, and XGBoost were utilized.

## Results
The XGBoost model showed good predictive accuracy with a root mean squared error (RMSE) of 4. Out of the total 50 features, only 8 had significant influence on the target variable. Diagnostic plots helped identify outliers and assess the normal distribution of errors.

## Areas of Focus
- Handling missing values: Missing iterative imputer was used to address missing values in the dataset.
- Time series cross-validation: Time series cross-validation was employed to evaluate the model's performance on unseen future data.

For more details and code, please visit [reesujagan42.github.io](https://reesujagan42.github.io). 

## Contact Information
Reesu Jagan  
Email: reesujagan42@gmail.com
