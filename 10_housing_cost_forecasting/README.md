# Housing cost forecasting

## Description of the project

In a project, we need to train a linear regression model on California housing data in 1990. Based on the data, we need to predict the median value of a house in a residential area. We will train the model and make predictions on the test set. To assess the quality of the model, we use the RMSE, MAE and R2 metrics.

## Description of data

The dataset columns contain the following data:
- `longitude` - latitude
- `latitude` - longitude
- `housing_median_age` - median age of residents of the residential area
- `total_rooms` - the total number of rooms in the houses of the residential area
- `total_bedrooms` - the total number of bedrooms in the houses of the residential area
- `population` - the number of people who live in the residential area
- `households` - the number of households in the residential area
- `median_income` - median income of residents of the residential area
- `median_house_value` - median cost of a house in a residential area
- `ocean_proximity` - proximity to the ocean

Based on the data, we need to predict the median cost of a house in a residential area - `median_house_value`

## Tools used

`pandas` `numpy` `spark` `seaborn` `sklearn` `math`

## Models used

`LinearRegression`

## Addition tools

`StringIndexer` `VectorAssembler` `OneHotEncoder` `pipelines` `folium` `h3` `geopandas` 

## Metrics

`RMSE` `MAE` `r2_score`
