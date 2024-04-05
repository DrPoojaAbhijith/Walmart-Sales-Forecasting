# Walmart-Sales-Forecasting

![image](https://github.com/DrPoojaAbhijith/Walmart-Sales-Forecasting/assets/160575120/d16d6c9d-e5fe-4398-8822-213b478e5d2e)

Description:
One of the leading retail stores in the US, Walmart, would like to predict the sales and demand accurately. There are certain events and holidays which impact sales on each day. There are sales data available for 45 stores of Walmart. The business is facing a challenge due to unforeseen demands and runs out of stock some times, due to the inappropriate machine learning algorithm. An ideal ML algorithm will predict demand accurately and ingest factors like economic conditions including CPI, Unemployment Index, etc.

Walmart runs several promotional markdown events throughout the year. These markdowns precede prominent holidays, the four largest of all, which are the Super Bowl, Labour Day, Thanksgiving, and Christmas. The weeks including these holidays are weighted five times higher in the evaluation than non-holiday weeks. Part of the challenge presented by this competition is modeling the effects of markdowns on these holiday weeks in the absence of complete/ideal historical data. Historical sales data for 45 Walmart stores located in different regions are available.

Dataset Info:\ This is the historical data that covers sales from 2010-02-05 to 2012-11-01, in the file Walmart_Store_sales. Within this file you will find the following fields:\

* Store - the store number
* Date - the week of sales
* Weekly_Sales - sales for the given store
* Holiday_Flag - whether the week is a special holiday week 1 – Holiday week 0 – Non-holiday week
* Temperature - Temperature on the day of sale
* Fuel_Price - Cost of fuel in the region
* CPI – Prevailing consumer price index
* Unemployment - Prevailing unemployment rate

 The walmart.csv contains 6435 rows and 8 columns.


Acknowledgements
The dataset is taken from Kaggle.

Problem Statement 1:
A retail store that has multiple outlets across the country are facing issues in managing the inventory - to match the demand with respect to supply.



Objective:¶
1. Understand the Dataset & cleanup (if required) in which it is provided with the weekly sales data for their various outlets. Use statistical analysis, EDA, outlier analysis, and handle the missing values to come up with various
insights that can give them a clear perspective on the following:
  a. If the weekly sales are affected by the unemployment rate, if yes - which stores
     are suffering the most?
  b. If the weekly sales show a seasonal trend, when and what could be the reason?
  c. Does temperature affect the weekly sales in any manner?
  d. How is the Consumer Price index affecting the weekly sales of various stores?
  e. Top performing stores according to the historical data.
  f. The worst performing store, and how significant is the difference between the
     highest and lowest performing stores.
2. Use predictive modeling techniques to forecast the sales for each store for the next 12 weeks

Stractegic Plan of Action:
We aim to solve the problem statement by creating a plan of action, Here are some of the necessary steps:

1. Data Exploration
2. Exploratory Data Analysis (EDA)
3. Data Pre-processing
4. Data Manipulation
5. Feature Selection/Extraction
6. Predictive Modelling
7. Project Outcomes & Conclusion
