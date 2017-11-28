# Bitcoin-Price-Time-Series-Forecasting
This project was done to predict the Bitcoin's price trend from Nov 2017 to Feb 2018. It’s a complicated task to predict a future selling price of a stock because there are many factors that can influence the price of a given stock. But I’ll try to see if I can at least get a sense of its trend in the next three months.

First, I downloaded the data from CoinMarketCap website. The data shows the Bitcoin’s close price (the price at 23:59:59 of each day) and the time frame is from April 2013 to November 2017.

Then, I tried to see if I could use ARIMA model, the most general class of models for forecasting a time series, for my forecasting. After using Dickey-Fuller test it turned out that the price data is not stationary and it’s very complicated to make it stationary. So I started to search to see if there are other models or packages that can be used for my case.

After some research I came across Prophet, an open source forecasting tool developed by Facebook. Prophet is based on an additive model where non-linear trends are fit with yearly and weekly seasonality, plus holidays. It works best with daily periodicity data with at least one year of historical data. Prophet is robust to missing data, shifts in the trend, and large outliers and it can be done in few lines of code. 

To see how it works please checkout my code.

