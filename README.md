![allstate](https://user-images.githubusercontent.com/19572673/62312597-8e5d9780-b45c-11e9-84d5-ba8994ccb7f7.jpg)
# Allstate Purchase Prediction Challenge
### Pujan Malavia

### Abstract:
As a customer shops an insurance policy, he/she will receive a number of quotes with different coverage options before purchasing a plan. This is represented in this challenge as a series of rows that include a customer ID, information about the customer, information about the quoted policy, and the cost. Predict the purchased coverage options using a limited subset of the total interaction history. If the eventual purchase can be predicted sooner in the shopping window, the quoting process is shortened and the issuer is less likely to lose the customer's business. Using a customer’s shopping history, can you predict what policy they will end up choosing? 

https://www.kaggle.com/c/allstate-purchase-prediction-challenge/overview

https://www.allstate.com/

### Industry: 
Insurance

### Company Information:
The Allstate Corporation is one of the largest insurance providers in the United States and one of the largest that is publicly held. The company also has personal lines insurance operations in Canada. Allstate was founded in 1931 as part of Sears, Roebuck and Co., and was spun off in 1993.The company has had its headquarters in Northfield Township, Illinois, near Northbrook since 1967. Allstate ranked No. 79 in the 2018 Fortune 500 list of the largest United States corporations by total revenue. Its current advertising campaign, in use since 2004, asks, "Are you in good hands?" 
##### https://en.wikipedia.org/wiki/Allstate

### Use Case:
Predict Bodily Injury Liability Insurance claim payments based on the characteristics of the insured’s vehicle

### Initial Dataset(s):

sampleSubmission.csv

test_v2.csv

train.csv

### Software:

Python

### Data:
The training and test sets contain transaction history for customers that ended up purchasing a policy. For each customer_ID, you are given their quote history. In the training set you have the entire quote history, the last row of which contains the coverage options they purchased. In the test set, you have only a partial history of the quotes and do not have the purchased coverage options. These are truncated to certain lengths to simulate making predictions with less history (higher uncertainty) or more history (lower uncertainty).

For each customer_ID in the test set, you must predict the seven coverage options they end up purchasing.

What is a customer?
Each customer has many shopping points, where a shopping point is defined by a customer with certain characteristics viewing a product and its associated cost at a particular time.

Some customer characteristics may change over time (e.g. as the customer changes or provides new information), and the cost depends on both the product and the customer characteristics.
A customer may represent a collection of people, as policies can cover more than one person.
A customer may purchase a product that was not viewed!
Product Options
Each product has 7 customizable options selected by customers, each with 2, 3, or 4 ordinal values possible:

Product Options

A product is simply a vector with length 7 whose values are chosen from each of the options listed above. The cost of a product is a function of both the product options and customer characteristics.

### Data Fields:

customer_ID - A unique identifier for the customer

shopping_pt - Unique identifier for the shopping point of a given customer

record_type - 0=shopping point, 1=purchase point

day - Day of the week (0-6, 0=Monday)

time - Time of day (HH:MM)

state - State where shopping point occurred

location - Location ID where shopping point occurred

group_size - How many people will be covered under the policy (1, 2, 3 or 4)

homeowner - Whether the customer owns a home or not (0=no, 1=yes)

car_age - Age of the customer’s car

car_value - How valuable was the customer’s car when new

risk_factor - An ordinal assessment of how risky the customer is (1, 2, 3, 4)

age_oldest - Age of the oldest person in customer's group

age_youngest - Age of the youngest person in customer’s group

married_couple - Does the customer group contain a married couple (0=no, 1=yes)

C_previous - What the customer formerly had or currently has for product option C (0=nothing, 1, 2, 3,4)

duration_previous -  how long (in years) the customer was covered by their previous issuer

A,B,C,D,E,F,G - the coverage options

cost - cost of the quoted coverage options

### Data Curation Process

R Visualization (ggplot2 & Maps libraries)

Number of Shopping Points

![viz1](https://user-images.githubusercontent.com/19572673/86279846-b42d7800-bba8-11ea-8633-d35253b49793.png)

Effect of Number of Shopping Points on Predictive Power of Last Quote

![viz2](https://user-images.githubusercontent.com/19572673/86279849-b4c60e80-bba8-11ea-8798-574ca5049fa9.png)

Effect of Purchase Hour on Likelihood of Changing from Last Quote

![viz3](https://user-images.githubusercontent.com/19572673/86279851-b4c60e80-bba8-11ea-9497-95d3cf4ba903.png)

Liklihood Selection of Option D based on Option C

![viz4](https://user-images.githubusercontent.com/19572673/86279852-b4c60e80-bba8-11ea-8ca0-991f9c3f0557.png)

Clustering of States

![viz5](https://user-images.githubusercontent.com/19572673/86279854-b4c60e80-bba8-11ea-9bfd-c4d5676bbc2f.png)

