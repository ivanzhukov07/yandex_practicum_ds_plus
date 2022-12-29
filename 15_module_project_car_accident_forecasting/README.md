# Сar accidentf orecasting

## Description of the project

It is necessary to create a system that could assess the risk of an accident along the chosen route.
Risk is the probability of an accident with any damage to the vehicle.
Once a driver has booked a car, got behind the wheel, and chosen a route, the system must assess the level of risk.
If the risk level is high, the driver will see a warning and route recommendations.

Current task is to understand whether it is possible to predict accidents based on historical data from one of the regions.

*The idea of solving the problem from the customer:*

   1. Create an accident prediction model (target value is **at_fault** in the **parties** table)
         - For the model, select the type of culprit - only car (**car**).
         - Select cases where the accident resulted in any damage to the vehicle, except for the **SCRATCH** type (scratch).
         - For modeling, limit yourself to data for **2012** - they are the most recent.
         - A prerequisite is to take into account the factor of the age of the car.
   2. Based on the model, explore the main factors of an accident
   3. Understand whether the results of modeling and analysis of the importance of factors will help answer the questions:
         - Is it possible to create an adequate driver risk assessment system when issuing a car?
         - What other factors should be taken into account?
         - Do we need to equip the car with any sensors or a camera?

## Description of data

**Collisions** — general information about the accident
    - Has a unique case_id.
    - This table describes general information about accidents. For example, where did it happen and when.

**Parties** — information about participants in the accident
    - Has a non-unique case_id that maps to the corresponding collision in the collisions table.
    - Each line here describes one of the parties involved in the accident.
    - If two cars collided, there should be two rows in this table with matching case_id.
    - If you need a unique ID, it's case_id and party_number.

**Vehicles** - information about affected vehicles
    - Has non-unique case_id and non-unique party_number that map to the collisions table and the parties table.
    - If you need a unique ID, it's case_id and party_number.

**Target feature**

`at_fault` in the *parties* table

## Tools used

`sqlalchemy` `pandas` `numpy` `matplotlib` `seaborn` `sklearn` `math`

## Models used

`DecisionTreeClassifier` `RandomForestClassifier` `CatBoostClassifier`

## Addition tools

`StandardScaler` `GridSearchCV` `cross_val_score` `confusion_matrix`

## Metrics

`recall_score` `precision_score`
