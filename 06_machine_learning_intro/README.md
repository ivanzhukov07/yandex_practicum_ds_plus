# Tariff recommendation

## Description of the project

It is necessary to build a system capable of assessing the behavior of customers who have not changed tariff plans for a long time, and offer users new tariffs that meet their preferences. There is data on visiting customers who have already switched to these tariffs. It is necessary to build a model for solving the problem, which will choose the appropriate coefficient. Data preprocessing is not usual, because was made as part of another project.

## Description of data

* `calls` - number of calls
* `minutes` - total duration of calls in minutes
* `messages` - number of sms messages
* `mb_used` - used Internet traffic in Mb
* `is_ultra` - what tariff did you use during the month ("Ultra" - **1**, "Smart" - **0**)


## Tools used

`pandas` `numpy` `matplotlib` `sklearn` `math`

## Models used

`DecisionTreeClassifier` `LogisticRegression` `RandomForestClassifier`

## Metrics

`accuracy_score`
