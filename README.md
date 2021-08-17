# Investment-and-Trading-Capstone-Project

## Project Motivation
Having worked in the financial industry for quite some time now, I was curious to see how stock prices changes with economical factors and interested in predicting stock prices. Also given the world wide lockdown due to the pandemic, I was really interested in investigating how the pandemic affected the prices of stock and which companies where able to bounce back quickly and how they compared to others.

## Project Overview
In this project, I will be building a stock price predictor that takes daily trading data over a certain date range as input, and outputs projected estimates for given query dates. Note that the inputs will contain multiple metrics, such as opening price (Open), highest price the stock traded at (High), how many stocks were traded (Volume) and closing price adjusted for stock splits and dividends (Adjusted Close); your system only needs to predict the Adjusted Close price.

In this project, I will be building a stock price predictor that takes daily trading data over a certain date range as input, and outputs projected estimates for given query dates. Note that the inputs will contain multiple metrics, such as opening price (Open), highest price the stock traded at (High), how many stocks were traded (Volume) and closing price adjusted for stock splits and dividends (Adjusted Close); your system only needs to predict the Adjusted Close price.

First of all, I did some exploratory analysis and visualization of the data to understand the data better. Some of the statistics that I investigated includes: cummulative returns, rolling means, Bollinger bands and daily returns which helped me to understand the volatility (risky) of stock prices. In the modelling section, I predicted Adjusted close value of Microsoft and Google stocks using three different models and compared their performance to each other.

 ## File Description
 This project has the following files:
 1. **fin_data.csv:** This contains data for different stocks from [yahoo finance](https://finance.yahoo.com/) which is located in the data folder.
 2. **investment_trading_capstone_project.ipynb:** This is the jupyter notebook containing the code for the project.


### Acknowledgment
Many thanks to Udacity for giving me an opportunity to try out real world problems and referencing the [Machine Learning for Trading course](https://www.udacity.com/course/machine-learning-for-trading--ud501) that gave me some insights into trading. Thanks to the Data Scientists who have inspired and provided insights to me through Github and StackOverflow.

This project was completed as part of the [Udacity Data Scientist Nanodegree](https://www.udacity.com/course/data-scientist-nanodegree--nd025) program.
