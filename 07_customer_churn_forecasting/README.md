# Customer churn

## Description of the project

Customers began to leave Beta-Bank. Every month. A little, but noticeable. Banking marketers figured it was cheaper to keep current customers than to attract new ones.

It is necessary to predict whether the client will leave the bank in the near future or not. You are provided with historical data on customer behavior and termination of agreements with the bank.

Build a model with an extremely large *F1*-score. To pass the project successfully, you need to bring the metric to 0.59. Check the *F1*-score on the test set yourself.

Additionally measure *AUC-ROC*, compare its value with *F1*-score.

Data source: [https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)

## Description of data

- `RowNumber` - row index in the data
- `CustomerId` - unique customer ID
- `Surname` - surname
- `CreditScore` — credit score
- `Geography` - country of residence
- `Gender` - gender
- `Age` - age
- `Tenure` - how many years a person has been a client of the bank
- `Balance` — account balance
- `NumOfProducts` - the number of bank products used by the client
- `HasCrCard` - the presence of a credit card
- `IsActiveMember` - client activity
- `EstimatedSalary` — estimated salary

**Target feature**

- `Exited` - the fact that the client left

## Tools used

`pandas` `numpy` `matplotlib` `sklearn` `math`

## Models used

`DecisionTreeClassifier` `LogisticRegression` `RandomForestClassifier`

## Addition tools

`StandardScaler` `upsample` `downsample`

## Metrics

`confusion_matrix` `f1_score` `roc_auc_score` `roc_curve`
