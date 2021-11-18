# fraud_detection
Fraud detection for e-commerce 

## Problem Statement
Company XYZ is an e-commerce site that sells hand-made clothes. You have to build a model that predicts whether a user has a high probability of using the site to perform some illegal activity or not. 

You only have information about the user first transaction on the site and based on that you have to make your classification ("fraud/no fraud"). 

TASKS:

a) For each user, determine her country based on the numeric IP address. 

b) Build a model to predict whether an activity is fraudulent or not.

## Data Description

a) Fraud_Data - information about each user first transaction 

Columns: 

user_id : Id of the user. Unique by user 

signup_time : the time when the user created her account (GMT time) 

purchase_time : the time when the user bought the item (GMT time) purchase_value : the cost of the item purchased (USD) 

device_id : the device id. You can assume that it is unique by device. I.e., transactions with the same device ID means that the same physical device was used to buy 

source : user marketing channel: ads, SEO, Direct (i.e. came to the site by directly typing the site address on the browser)

browser : the browser used by the user. 

sex : user sex: Male/Female 

age : age of user

user age ip_address : user numeric ip address 

class : this is what we are trying to predict: whether the activity was fraudulent (1) or not (0).


b) IpAddress_to_Country - mapping each numeric ip address to its country. 

For each country, it gives a range. If the numeric ip address falls within the range, then the ip address belongs to the corresponding country. 

Columns: 

lower_bound_ip_address : the lower bound of the numeric ip address for that country 

upper_bound_ip_address : the upper bound of the numeric ip address for that country 

country : the corresponding country. If a user has an ip address whose value is within the upper and lower bound, then she is based in this country.
