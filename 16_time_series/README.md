# The number of taxi orders for the next hour forecasting

## Description of the project

The company collected historical data on taxi orders at airports. To attract more drivers during peak load, you need to predict the number of taxi orders for the next hour. Build a model for such a prediction. The value of the RMSE metric in the test sample should be no more than 48

## Description of data

`num_orders` - target variable, set by condition

## Tools used

`TimeSeriesSplit` `catboost` `lightgbm` `statsmodels` `sklearn` `pandas` `numpy` `matplotlib` `math` `time`

## Models used

`LGBMRegressor` `CatBoostRegressor` `LinearRegression` `RandomForestRegressor`

## Addition tools

`TimeSeriesSplit` `seasonal_decompose` `StandardScaler` `GridSearchCV`

## Metrics

`MSE` `RMSE`