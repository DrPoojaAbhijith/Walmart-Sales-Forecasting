# Walmart-Sales-Forecasting

![image](https://github.com/DrPoojaAbhijith/Walmart-Sales-Forecasting/assets/160575120/d16d6c9d-e5fe-4398-8822-213b478e5d2e)

Table Of Contents
Problem Statement
Project Objective
Data Description
Data Pre-processing steps and inspiration
Choosing the algorithm for the project
Motivation and reasons for choosing the algorithm
Assumptions
Model evaluations and techniques
Inferences from the same
Future possibilities of the project
Conclusion
References
Problem Statement
A retail store that has multiple outlets across the country are facing issues in managing the inventory - to match the demand with respect to supply.  

Project Objective
You are provided with the weekly sales data for their various outlets. Use statistical analysis, EDA, outlier analysis, and handle the missing values to come up with various insights that can give them a clear perspective on the following: a. If the weekly sales are affected by the unemployment rate, if yes - which stores are suffering the most? b. If the weekly sales show a seasonal trend, when and what could be the reason? c. Does temperature affect the weekly sales in any manner? d. How is the Consumer Price index affecting the weekly sales of various stores? e. Top performing stores according to the historical data. f. The worst performing store, and how significant is the difference between the highest and lowest performing stores.
Use predictive modeling techniques to forecast the sales for each store for the next 12 weeks.  
Data Description
Feature Name Description Store Store number Date Week of sales Weekly_Sales Sales for the given store in that week Holiday_Flag If it is a holiday week Temperature Temperature on the day of the sale Fuel_Price Cost of the fuel in the region CPI Consumer Price Index Unemployment Unemployment Rate

 

Data Pre-processing steps and inspiration
Loading the Dataset: The initial step involves loading the dataset into the analysis environment, typically using libraries like Pandas in Python, ensuring accessibility for further examination.

Checking for Data Types: It is imperative to inspect the data types of each column to ensure consistency and appropriateness for subsequent analyses and operations.

Converting Date Column: When dealing with temporal data, such as dates, converting the date column from an object type to a date type facilitates time-based analyses and visualizations.

Handling Outliers: Identification and treatment of outliers are crucial to maintain data integrity. Outliers are assessed visually through plots or statistically using methods like z-scores or IQR (Interquartile Range), ensuring their handling aligns with the context and domain knowledge.

Correlation Analysis: Utilizing tools like heatmaps aids in understanding the interrelationships between various features within the dataset, providing insights into potential dependencies and guiding further exploration.

Exploring Relationships: Beyond correlation analysis, exploring relationships between columns through visualizations and statistical methods unveils additional patterns and dependencies, enriching the understanding of the dataset's dynamics.

Time Series Analysis: Conducting time series analysis involves assessing stationarity through techniques like examining rolling mean and standard deviation, essential for ensuring the reliability of subsequent forecasting models.

Forecasting Models Selection: Employing forecasting model ARIMA entails a methodical approach based on the dataset's characteristics and the desired level of complexity, enabling accurate prediction of future trends.

These pre-processing steps and methodologies lay a solid foundation for rigorous data analysis and forecasting, contributing to informed decision-making and actionable insights.  

Choosing the algorithm for the project
I am employing ARIMA model to conduct forecast analysis on the provided dataset. These methods offer diverse perspectives for predicting future trends and patterns within the data. ARIMA integrates autoregressive, moving average, and differencing components to capture complex temporal dynamics. By leveraging these techniques, I aim to generate accurate forecasts that inform decision-making and strategic planning. The model facilitates a comprehensive understanding of the dataset's predictive capabilities.

 

Motivation and reasons for choosing ARIMA MODEL
The choice of algorithm for forecast analysis was motivated by its distinct strengths and suitability for different aspects of the dataset. Stationarity: ARIMA works well with stationary data or can be made stationary through differencing. Autocorrelation: ARIMA captures autocorrelation with AR and MA components. Flexibility: ARIMA handles various patterns like trend and seasonality. Simple Structure: It's easier to interpret and implement compared to some other models. Forecasting Accuracy: ARIMA provides accurate forecasts for many real-world datasets. Diagnostic Tools: ARIMA models come with diagnostic tools such as residual analysis, ACF (Autocorrelation Function) and PACF (Partial Autocorrelation Function) plots, which help assess the model's adequacy and identify any remaining patterns in the residuals. By employing ARIMA MODEL, I aim to leverage its complementary strengths to generate robust and accurate forecasts that inform decision-making processes effectively.  

Assumptions
No Assumptions made  

Inferences from the same
• Inferences from EDA Part I Have Done EDA based on the concept of independent variable’s v/s dependent variable (Weekly Sales).

Store V/s Weekly Sales (Top 10 and Worst 10 Stores) Top 10 Performance Stores The Stores 4,20,14 is having the highest sales in top 10 stores segment. The Stores 6,39 is having the Lowest sales in top 10 stores segment. Worst Performance 10 Stores The Stores 29,16,37 is having the highest sales in Bottom 10 stores segment The Stores 33,44 is having the highest sales in Bottom 10 stores segment.

Holidays V/s Weekly Sales The Sales are High in Normal Days, it is Quite common because of that holiday are always low compared to working days.

Date V/s Weekly Sales Weekly Sales most of weeks are consolidating expect some quarters which are in winter season is having seasonal spikes

Temperature V/s Weekly Sales Stores perform well in moderate temp that is 26-50. Sales went peaks in Moderate to High temp that is 51-75. Sales went down in Very High and Low temp that is 0-25 & 76-100.

Fuel Price V/s Weekly Sales When the fuel prices are moderate the performance of stores are also moderately high. But the fuel Price went above the moderate level that is 3.5, and the sales are also went very High. May be the Inflation and fear of increasing prices people are bought more grocery to mitigate with inflation. and when fuel price went even high the purchase power of people went down. may be the inflation and increasing in goods price.

CPI V/s Weekly Sales when inflation is lower the performance of stores are high. in initial time of inflation, the sale was drop significantly. in third level when inflation is high the people may scare for future prices and bought more grocery for future needs also. eventually when the inflation went peaks the sales are went down.

Unemployment V/s Weekly Sales When the Unemployment rate is between the 6 to 10 the stores are performing well. But whenever the Unemployment rate is increasing the sales went down.

Correlation analysis between variables Quarters and Fuel Price having high correlation. Because the fuel prices are also depended on the seasonal changes.

• Inferences from Questioner Part
a) If the weekly sales are affected by the unemployment rate, if yes - which stores are suffering the most?
I Consider the Top 5 Suffering Stores Only. And listed below

![Top 5 Stores](image

b) If the weekly sales show a seasonal trend, when and what could be the reason?
![Weekly Sales Trend Component] (image

• Regarding the Temperature data, a seasonal downward trend is observed starting from September 2010 until January 2011. Subsequently, there's a gradual increase. However, from September 2011, temperatures start to decline again.

• In the Weekly Sales Data, there is a noticeable increase in sales starting from September 2010, followed by a seasonal upward trend until January 2011. Afterward, the sales stabilize, eventually transitioning to a downward trend. This pattern is repeated from September 2011 to January 2012.

• In summary, there appears to be an inverse relationship between Temperature and Weekly Sales. When temperatures decrease, weekly sales tend to rise, and vice versa. This inverse correlation is evident from September 2011 to January 2012, as well as from September 2011 to January 2012.

c) Does temperature affect the weekly sales in any manner?
There is a negatively correlation between the temperature and weekly sales so, the answer for question c: Yes, there is a Negative correlation and the Temperature is affecting the Weekly Sales

d) How is the Consumer Price index affecting the weekly sales of various stores?
There is a negative correlation between the CPI and weekly sales so, the answer for question D: Yes, there is a Negative correlation and the CPI is affecting the Weekly Sales we can see that in below graph as well. when the CPI increasing the sales are down

e) Top performing stores according to the historical data.
The Stores 4,20,14 is having the highest sales in top 10 stores segment The Stores 6,39 is having the Lowest sales in top 10 stores segment

f) The worst performing store, and how significant is the difference between the highest and lowest performing stores.
The Stores 29,16,37 is having the highest sales in Bottom 10 stores segment. The Stores 33,44 is having the highest sales in Bottom 10 stores segment.

 

Conclusion
Based on the analysis conducted on the dataset, it can be concluded that the ARIMA model is the most suitable for forecasting purposes.

Its simplicity and ability to effectively smooth out noise make it particularly well-suited for this dataset.
Its straightforward methodology and robust performance make it a reliable choice for generating forecasts.
And the model accuracy was also quite good. And its near to 0
model accuracy for all the stores is Root Mean Squared Error 0.09083478416569807
model accuracy for Store 1 Root Mean Squared Error 0.08634807425384945
accuracy for Store 6 Root Mean Squared Error 0.11624010402978888
model accuracy for Store 11 Root Mean Squared Error 0.10223844724990286
model accuracy for Store 17 Root Mean Squared Error 0.1049818692897262
And the model accuracy for Store 33 Root Mean Squared Error 0.07536825631037113
REFERENCES
Open AI. (n.d.). ChatGPT.
