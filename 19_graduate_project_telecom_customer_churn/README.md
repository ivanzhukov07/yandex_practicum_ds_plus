# Graduate project
# Telecom. Customer churn forecasting

## Description of the project

A telecom operator wants to learn how to predict customer churn.
If it turns out that the user plans to leave, he will be offered promotional codes and special conditions. The operator's team collected personal data about some customers, information about their tariffs and contracts.

### Description of services

The operator provides two main types of services:
- Fixed telephone connection. It is possible to connect a telephone set to several lines at the same time
- Internet. The connection can be of two types: via a DSL telephone line (from the English *digital subscriber line* - "digital subscriber line") or fiber optic cable (*Fiber optic*)

The following services are also available:
- Internet security: antivirus (*DeviceProtection*) and blocking of unsafe sites (*OnlineSecurity*)
- Dedicated technical support line (*TechSupport*)
- Cloud file storage for data backup (*OnlineBackup*)
- Streaming TV (*StreamingTV*) and movie catalog (*StreamingMovies*)

Clients can pay for services every month or sign a contract for 1-2 years. Various payment methods and the possibility of receiving an electronic receipt for services are available

## Description of data

Information about contracts is current as of February 1, 2020.

The data is stored in tables in a PostgreSQL database:
- `contract` — information about the contract
- `personal` - personal data of the client
- `internet` - information about Internet services
- `phone` — information about telephony services

**Target feature**

- `isCanceled` — order cancellation

## Tools used

`sqlalchemy` `pandas` `numpy` `matplotlib` `seaborn` `sklearn` `pytorch` `math`

## Models used

`LGBM` `CatBoost` `RandomForestClassifier` `neural network`

## Addition tools

`StandardScaler` `GridSearchCV` `cross_val_score` `confusion_matrix`

## Metrics

`roc_auc_score` `accuracy_score`