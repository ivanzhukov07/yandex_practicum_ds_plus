# Determination of a prospective tariff for a telecom company

## Description of the project

You are an analyst at Megaline, a federal mobile operator. Clients are offered two tariff plans: "Smart" and "Ultra". To adjust the advertising budget, the commercial department wants to understand which tariff brings in more money.
You have to make a preliminary analysis of tariffs on a small sample of customers. At your disposal are the data of 500 Megaline users: who they are, where they are from, what tariff they use, how many calls and messages each sent in 2018. It is necessary to analyze the behavior of customers and draw a conclusion - which tariff is better.

## Description of tariffs

**Tariff "Smart"**
- Monthly fee: `550` rubles
- Included `500 minutes` conversation, `50` messages and `15 GB` internet traffic
- The cost of services above the tariff package:
    1. minute of conversation: `3 rubles`
    2. message: `3 rubles`;
    3. 1 GB of Internet traffic: `200 rubles`

**Tariff "Ultra"**
- Monthly fee: `1950` rubles
- Included `3000 minutes` conversation, `1000` messages and `30 GB` internet traffic
- The cost of services above the tariff package:
    1. minute of conversation: `1 ruble`;
    2. message: `1 ruble`;
    3. 1 GB of Internet traffic: `150 rubles`
    
 
## Description of data

**users** table (user information):
* `user_id` - unique user ID;
* `first_name` - username;
* `last_name` - user's last name;
* `age` - user's age (years);
* `reg_date` — tariff connection date (day, month, year);
* `churn_date` — date when the tariff was discontinued (if the value is omitted, then the tariff was still in effect at the time of data upload);
* `city` - user's city of residence;
* `tarif` — tariff plan name;

**messages** table (message information):
* `id` — unique message number;
* `message_date` — message date;
* `user_id` - identifier of the user who sent the message;

Table **internet** (information about Internet sessions):
* `id` - unique session number;
* `mb_used` - the amount of Internet traffic spent per session (in megabytes);
* `session_date` - Internet session date;
* `user_id` - user ID;

**tariffs** table (tariff information):
* `tariff_name` — tariff name;
* `rub_monthly_fee` — monthly subscription fee in rubles;
* `minutes_included` - the number of minutes of conversation per month included in the subscription fee;
* `messages_included` - the number of messages per month included in the subscription fee;
* `mb_per_month_included` - the amount of Internet traffic included in the subscription fee (in megabytes);
* `rub_per_minute` - the cost of a minute of conversation in excess of the tariff package (for example, if the tariff includes 100 minutes of conversation per month, then a fee will be charged from 101 minutes);
* `rub_per_message` - the cost of sending a message in excess of the tariff package;
* `rub_per_gb` - the cost of an additional gigabyte of Internet traffic in excess of the tariff package (1 gigabyte = 1024 megabytes).
      

## Tools used

`pandas` `numpy` `matplotlib` `math`
