# Determining cars cost

## Description of the project

The service for the sale of used cars is developing an application to attract new customers. In it, you can quickly find out the market value of your car. Historical data is at your disposal: technical specifications, complete sets and prices of cars. You need to build a model to determine the cost. 

**Important to the customer:**

- prediction quality
- prediction speed
- training time

## Description of data

**Features**

- `DateCrawled` — date of downloading the questionnaire from the database
- `VehicleType` — car body type
- `RegistrationYear` — year of registration of the car
- `Gearbox` — type of gearbox
- `Power` — power (hp)
- `Model` — car model
- `Kilometer` — mileage (km)
- `RegistrationMonth` — month of car registration
- `FuelType` — fuel type
- `Brand` — car brand
- `NotRepaired` — was the car under repair or not
- `DateCreated` — date the questionnaire was created
- `NumberOfPictures` — number of photos of the car
- `PostalCode` — postal code of the questionnaire owner (user)
- `lastSeen` — date of the user's last activity

**Target**

- `Price` — price (Euro)


## Tools used

`catboost` `lightgbm` `sklearn` `pandas` `numpy` `matplotlib` `math` `time`

## Models used

`CatBoostRegressor` `LGBMRegressor` `DecisionTreeRegressor` `RandomForestRegressor` `LinearRegression`

## Addition tools

`OneHotEncoder` `OrdinalEncoder` `StandardScaler` `GridSearchCV`

## Metrics

`mean_squared_error`
