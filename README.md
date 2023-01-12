# Yes-Bank-Stock-Closing-Prediction

## Problem Statement
In the Indian financial sector, Yes Bank is well known for its modern-day systems, including its financial markets. It has been in the news since 2018 due to the fraud case involving Rana Kapoor. Therefore, it was interesting to observe how this affected the stock price of the company. As well as this, it was interesting to see whether any other predictive models can be used to account for such situations. Since the bank's inception, this dataset contains monthly stock prices, including closing, starting, highest and lowest prices of every month. The main objective is to predict the closing price of the stock for the month.

## Introduction
The stock market is characterized as dynamic, unpredictable, and non-linear. Predicting stock prices is a challenging task as it depends on various factors, including but not limited to political conditions, global economy, company’s financial reports and performance, etc. Therefore, predicting the value of the stock in advance by analyzing the trend over the last few years could be beneficial for making stock market decisions to maximize profits and minimize losses. Traditionally, two main approaches have been proposed for estimating the stock price of an organization. The technical analysis method focuses on the historical prices of stocks, such as closing and opening prices, the volume traded adjacent to close values, etc. The stock is used to forecast the future price of the stock.

The second type of analysis is fundamental or qualitative, which is performed based on external factors like company profile, market situation, political and economic factors, textual information in the form of financial news articles, social media, and even blogs by economic analysts. Nowadays, advanced intelligent techniques based on technical or fundamental analysis are used to predict market prices. Particularly, for stock market analysis, the data size is enormous and non-linear. It is necessary to develop a model that can identify hidden patterns within this large dataset to deal with such a variety of data. Machine learning techniques in this field have proven to increase efficiency by 60-80 percent over the previous methodology.

## Steps involved

## 1. Data Preparation
Data preparation is the process of cleaning and transforming raw data before processing and analysis. It is an important step before processing and often involves reformatting data, making corrections to data, and combining data sets to enrich data.

## 2. Data observation and cleaning
Our dataset consists of 185 rows and 5 columns. The data type of Date is given as an object which we need to change to Date Time. As of July 2005, the bank's stock was listed on the stock exchange. We have data available from July 2005 to November 2020. The statistical information shows that it is not a normal distribution, since the mean and 50% values are very different, and there are no duplicates and no null values.

## 3. Exploratory Data Analysis
Exploratory data visualizations (EDVs) are the type of visualizations we assemble when we do not have a clue about what information lies within our dataset.

## 4. Data pre-processing
The date given in the data is in MMM-YY format and is converted to the appropriate date from YYYY-MM-DD. Since the "Date" column indicates the type of object, we have converted it into a date-time. As you can see from the chart below, the trend is upwards from 2009 to 2018, but thereafter the trend is downwards. This is due to the fraud involving Rana Kapoor Closing price of the stock price is always important, so we take the close price as a dependent variable.
 
## 5. Model building, Predictions, and Forecasting
A) Linear Regression - Linear regression is one of the simpler and more popular machine learning algorithms. This is a statistical methodology used for the Linear regression algorithm displays. linear relation between a dependant (y) (in this case is Close Price) and one or more.independent variables (in this case Open, Low, high), so-called linear regression.

B) Lasso regression - Lasso (absolute shrinkage minimum and select operator) is a regression analysis method that selects variables and adjusts them in sequence. improves the accuracy of forecasts and the consequent interpretability of the statistical model. When we have rolled out the outcome of the lasso regression model is given below table. Here We are valued at R-Square 94.96.

C) Ridge regression - Ridge regression is a model development method that is used for analyses of any data	that	suffers from multi-collinearity. This method carries out an adjustment L2. When the issue of multicollinearity occurs; least-squares are unbiased, and variances are large; this results in predicted values being far away from the actual values.

D) Elastic Net Regression - Elastic Net Regression is the third type of Regularization technique. It came into existence due to the limitation of the Lasso regression. Lasso regression cannot assume correct alpha and lambda values according to data requirements. The solution to this problem is to combine peak regression penalties with lasso regression penalties.

E) Cross Validation - Basically, Cross Validation is a technique using which a Model is evaluated on the dataset on which it is not trained, i.e. it can be a test data or can be another set as per availability or feasibility. In this case, the best parameter is alpha: 0.0014 and CV = 5. When cross-validating is deployed, the results from the lasso regression model are given below the table. Cross Validation for ridge regression, we found the best parameter 'alpha': 3 and CV= 5 and for elastic net also we found the best parameter 'alpha': 0.01 and CV= 5.

## Challenges
In deciding on the independent variables, we faced difficulties, as there were very limited parameters and they had very strong collinearity with the dependent variable. The downside to linear regression while predicting share prices is that it is very limited in scope. Many predictors cannot be used, which is necessary to resolve the price action prediction problem. From our observation, we concluded that such issues can be better addressed by using time series forecasting. Select the correct k nearest neighbor K.

## Conclusion
* From all the ml model used in this project, Linear regression has given best R2 score around 95.52%.
* The popularity of stock price volatility increases extremely quickly from day to day, encouraging researchers to find new methods in the event of fraud. This technique is used for prediction and is not only helpful to researchers to predict future stock closing prices or any fraud happen or not but also helps investors or any person who deals with the stock market in order to predict of model with good accuracy. As I mentioned at the beginning of the article, share prices are influenced by news about the business and other factors such as demonetization or mergers, or division of businesses.
* There are also some intangible factors that may often not be predictable in advance. Time series and fbpropfet is the best model for yes bank stock closing price data, this model is used for further prediction.






