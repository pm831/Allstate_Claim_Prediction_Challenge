![allstate](https://user-images.githubusercontent.com/19572673/62312597-8e5d9780-b45c-11e9-84d5-ba8994ccb7f7.jpg)
# Allstate Claim Prediction Challenge

## Abstract:
As a customer shops an insurance policy, he/she will receive a number of quotes with different coverage options before purchasing a plan. This is represented in this challenge as a series of rows that include a customer ID, information about the customer, information about the quoted policy, and the cost. Predict the purchased coverage options using a limited subset of the total interaction history. If the eventual purchase can be predicted sooner in the shopping window, the quoting process is shortened and the issuer is less likely to lose the customer's business. Using a customer’s shopping history, can you predict what policy they will end up choosing? https://www.kaggle.com/c/allstate-purchase-prediction-challenge/overview

## Company Information:
The Allstate Corporation is one of the largest insurance providers in the United States and one of the largest that is publicly held. The company also has personal lines insurance operations in Canada. Allstate was founded in 1931 as part of Sears, Roebuck and Co., and was spun off in 1993.The company has had its headquarters in Northfield Township, Illinois, near Northbrook since 1967. Allstate ranked No. 79 in the 2018 Fortune 500 list of the largest United States corporations by total revenue. Its current advertising campaign, in use since 2004, asks, "Are you in good hands?" https://en.wikipedia.org/wiki/Allstate

## Use Case:
### Predict Bodily Injury Liability Insurance claim payments based on the characteristics of the insured’s vehicle

## Initial Dataset:

## Software:
### Python

## Data:
Each row contains one year’s worth information for insured vehicles.  Since the goal of this competition is to improve the ability to use vehicle characteristics to accurately predict insurance claim payments, the response variable (dollar amount of claims experienced for that vehicle in that year) has been adjusted to control for known non-vehicle effects. Some non-vehicle characteristics (labeled as such in the data dictionary) are included in the set of independent variables.  It is expected that no “main effects” corresponding will be found for these non-vehicle variables, but there may be interesting interactions with the vehicle variables. 

Calendar_Year is the year that the vehicle was insured.  Household_ID is a household identification number that allows year-to-year tracking of each household. Since a customer may insure multiple vehicles in one household, there may be multiple vehicles associated with each household identification number. "Vehicle" identifies these vehicles (but the same "Vehicle" number may not apply to the same vehicle from year to year). You also have the vehicle’s model year and a coded form of make (manufacturer), model, and submodel.  The remaining columns contain miscellaneous vehicle characteristics, as well as other characteristics associated with the insurance policy.  See the "data dictionary" (data_dictionary.txt) for additional information.

Our dataset naturally contained some missing values. Records containing missing values have been removed from the test data set but not from the training dataset. You can make use of the records with missing values, or completely ignore them if you wish. They are coded as "?".

There are two datasets to download: training data and test data. You will use the training dataset to build your model, and will submit predictions for the test dataset. The training data has information from 2005-2007, while the test data has information from 2008 and 2009. Submissions should consist of a CSV file. Records from 2008 will be used to score the leaderboard, and records from 2009 will be used to determine the final winner.
