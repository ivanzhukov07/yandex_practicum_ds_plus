# Churn forecasting and payback calculation

## Description of the project

To attract customers, this hotel chain has added to its website the ability to book a room without prepayment. However, if the customer cancelled the booking, the company suffered losses. The hotel staff could, for example, buy groceries for the arrival of a guest or simply not have time to find another client.  
To solve this problem, we need to develop a system that predicts the rejection of armor. If the model shows that the reservation will be canceled, the client is invited to make a deposit. The deposit amount is 80% of the room rate. The money will be debited from the client's account if he still cancels the reservation.

The profit of the hotel is the difference between the cost of a room for all nights and the cost of a one—time service: both during the preparation of the room and during the stay of the guest.  
The hotel has several types of rooms. Depending on the type of room, the cost per night is assigned. There are also cleaning costs. If the client has rented a room for a long time, then they are cleaned every two days.  

The hotel's pricing policy uses seasonal coefficients: in spring and autumn prices increase by 20%, in summer — by 40%.  

There is a budget for the development of the forecasting system — 400 000. At the same time, it should be taken into account that the implementation of the model should pay off.  Development costs should be less than the revenue that the system will bring to the company.

## Description of data

The *hotel_train* and *hotel_test* tables contain the same columns:

- `ADR` — average daily Room Rate
- `Adults` — number of adult guests
- `Agent` — the agent through whom the order was made
- `AssignedRoomType` — number type
- `Babies' — number of babies
- `BookingChanges` — the number of changes to the order parameters
- `Children` — the number of children from 3 to 14 years old
- `CompanyId` — ID of the company or legal entity responsible for booking
- `Country` — citizenship of the guest
- `CustomerType` — type of the customer:
    - `Contract` — contract with a legal entity
    - `Group` — group check-in
    - `Transient` — not related to the contract or group check
    - `Transient—party` - not related to the contract or group check-in, but related to the booking type `Transient`
- `DaysInWaitingList` — how many days the order was waiting for confirmation
- `DistributionChannel` — order distribution channel
- `IsRepeatedGuest` — indicates that the guest is booking a room for the second time
- `LeadTime` — the number of days between the booking date and the arrival date
    - `Meal` — ordering options:
    - `SC` — no additional options
    - `BB` — breakfast included
    - `HB` — breakfast and lunch included
    - `FB` — breakfast, lunch and dinner included
- `PreviousBookingsNotCanceled` — the number of confirmed orders from the client
- `PreviousCancellations` — the number of cancelled orders from the client
- `RequiredCarParkingSpaces` — the need for a place for the car
- `ReservedRoomType` — type of reserved room
- `StaysInWeekendNights` — number of nights on weekends
- `StaysInWeekNights` — number of nights on weekdays
- `TotalOfSpecialRequests` — number of special marks

**Target feature**

- `isCanceled` — order cancellation

## Tools used

`pandas` `numpy` `matplotlib` `seaborn` `sklearn` `math`

## Models used

`DecisionTreeClassifier` `LogisticRegression` `RandomForestClassifier`

## Addition tools

`StandardScaler` `GridSearchCV` `cross_val_score` `roc_curve`

## Metrics

`roc_auc_score` `precision_score` `recall_score`
