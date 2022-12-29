# Choosing a location for an oil well

## Description of the project

An oil company needs to decide where to drill a new well. To do this, it is necessary to build a model to determine the region where mining will bring the greatest profit. You also need to analyze the possible profit and risks.

## Description of data

Geological exploration data of the three regions are in different files.

- `id` - unique identifier of the well
- `f0`, `f1`, `f2` - three signs of points (it doesn't matter what they mean, but the signs themselves are significant)
- `product` - volume of reserves in the well (thousand barrels)


## Tools used

`sklearn` `scipy` `matplotlib` `pandas` `numpy`

## Models used

`LinearRegression`

## Addition tools

`bootstrap` `StandardScaler`

## Metrics

`r2_score` `mean_squared_error` `mean_absolute_error`
