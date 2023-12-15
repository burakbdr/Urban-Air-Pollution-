# Urban-Air-Pollution-
## PM 2.5 Concentration Level Prediction

This tool utilizes machine learning algorithms to predict global PM2.5 levels leveraging accessible satellite data (Sentinel 5P) and weather data (Global Forecast System - GFS). The predictions aim to provide reliable information to the World Health Organization for policy initiatives aimed at mitigating PM2.5 exposure worldwide.

### Methodology

The project focuses on predicting PM2.5 levels globally, which is essential for understanding and addressing urban air pollution. The tool utilizes various machine learning models, such as Random Forest, Gradient Boosting, Extra Trees, K-Nearest Neighbors, and Linear Regression, to predict PM2.5 levels based on satellite and weather data.

#### Model Stacking

The stacking technique is employed to combine multiple regression models for enhanced prediction accuracy. The following stacking approaches were explored:

- StackingRegressor: A stacking ensemble method is employed using various base regressors and a final estimator.
- RandomForestRegressor, LinearRegression, KNeighborsRegressor, GradientBoostingRegressor, ExtraTreesRegressor, and Ridge: These regressors are used as base models within the stacking ensemble.

#### Stacking Regressor 1

- **Models Used**: Linear Regression, K-Nearest Neighbors, Gradient Boosting, Extra Trees
- **Final Estimator**: Linear Regression
- **Evaluation Metrics**:
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R-squared (R²)
  - Adjusted R-squared


#### Stacking Regressor 2

- **Models Used**: Linear Regression, Extra Trees
- **Final Estimator**: Linear Regression
- **Evaluation Metrics**:
  - MSE
  - RMSE
  - R²
  - Adjusted R²


#### Stacking Regressor 3

- **Models Used**: Linear Regression, K-Nearest Neighbors, Gradient Boosting, Extra Trees
- **Final Estimator**: RandomForest
- **Evaluation Metrics**:
  - MSE
  - RMSE
  - R²
  - Adjusted R²


#### Stacking with Ridge Regression

- **Models Used**: Random Forest, K-Nearest Neighbors, Gradient Boosting, Extra Trees
- **Final Estimator**: Ridge Regression
- **Evaluation Metrics**:
  - MSE
  - RMSE
  - R²
  - Adjusted R²



## About PM 2.5

PM2.5 refers to atmospheric particulate matter that have a diameter of less than 2.5 micrometers and is one of the most harmful air pollutants.
These particles are a type of air pollution and can be composed of various materials, including dust, soot, smoke, organic chemicals, and metals.

PM2.5 is a common measure of air quality that normally requires ground-based sensors to measure.But ground based sensors are expensive and because of these PM 2.5 level can not be measured everywhere in the world. 

## Dataset

In the project Ground Based-Sensors in train data used as target and model trained with 5P Satellite Data and The Global Forecast System (GFS) data.

The Zindi Channel and Dataset: [Urban Air Pollution Challenge](https://zindi.africa/competitions/urban-air-pollution-challenge).

### Features

- [Weather Data](https://developers.google.com/earth-engine/datasets/catalog/NOAA_GFS0P25).
- [NO2: Offline Nitrogen Dioxide](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_NO2).
- [AER AI: Offline UV Aerosol Index](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_AER_AI).
- [SO2: Offline Sulfur Dioxide](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_SO2).
- [CH4: Offline Methane](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_CH4).
- [O3: Offline Ozone](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_O3).
- [CO: Offline Carbon Monoxide](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_CO).
- [HCHO: Offline Formaldehyde](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_HCHO).
- [CLOUD: Near Real-Time Cloud](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S5P_OFFL_L3_CLOUD).


## Requirements and Environment

Requirements:
- pyenv with Python: 3.11.3

Environment: 

```Bash
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```


