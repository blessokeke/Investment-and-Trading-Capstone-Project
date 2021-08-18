# Investment-and-Trading-Capstone-Project

## Project Motivation
Having worked in the financial industry for quite some time now, I was curious to see how stock prices changes with economical factors and interested in predicting stock prices. Also given the world wide lockdown due to the pandemic, I was really interested in investigating how the pandemic affected the prices of stock and which companies where able to bounce back quickly and how they compared to others.

## Project Overview
In this project, I will be building a stock price predictor that takes daily trading data over a certain date range as input, and outputs projected estimates for given query dates. Note that the inputs will contain multiple metrics, such as opening price (Open), highest price the stock traded at (High), how many stocks were traded (Volume) and closing price adjusted for stock splits and dividends (Adjusted Close); your system only needs to predict the Adjusted Close price.

In this project, I will be building a stock price predictor that takes daily trading data over a certain date range as input, and outputs projected estimates for given query dates. Note that the inputs will contain multiple metrics, such as opening price (Open), highest price the stock traded at (High), how many stocks were traded (Volume) and closing price adjusted for stock splits and dividends (Adjusted Close); your system only needs to predict the Adjusted Close price.

First of all, I did some exploratory analysis and visualization of the data to understand the data better. Some of the statistics that I investigated includes: cummulative returns, rolling means, Bollinger bands and daily returns which helped me to understand the volatility (risky) of stock prices. In the modelling section, I predicted Adjusted close value of Microsoft and Google stocks using three different models and compared their performance to each other.

## Installations
The following libraries are needed to successfully run this project. First of all you will need to install `yfinance` using `pip install yfinance`.
I used python 3 for this project and other packages installed are:

  1. statsmodels
  2. sklearn
  3. seaborn
  4. matplotlib
  5. pandas
  6. numpy
  7. keras


 ## File Description
 This project has the following files:
 1. **fin_data.csv:** This contains data for different stocks from [yahoo finance](https://finance.yahoo.com/) which is located in the data folder.
 2. **investment_trading_capstone_project_main.ipynb:** This is the jupyter notebook containing the code for the project.

## Results Summary
![image1](https://github.com/blessokeke/Investment-and-Trading-Capstone-Project/blob/main/images/prediction_list.PNG)
![image1](https://github.com/blessokeke/Investment-and-Trading-Capstone-Project/blob/main/images/prediction_plot.PNG)
![image1](https://github.com/blessokeke/Investment-and-Trading-Capstone-Project/blob/main/images/prediction_plot_google.PNG)

From my investigation of three different models, I observed that RandomForestRegressor delivered a much better results with a lower mean absolute error (0.05, 0.0008 for Microsoft and Google respectively) than the LinearRegression or the LSTM. I also observed that tunning the parameters for LSTM (e.g the number of epochs and batch_size) resulted in better prediction but this takes time and may not always be feasible.

When exploring the data, it was interesting to see how the stock prices of different companies changed due to the pandemic and how the technological companies stock prices bounced back more quickly than the other companies considered. It was also interesting to see how Pfizer stocks improved as the vaccine rollout began.

Here are some major highlights from the data exploration section:
  1. 2019: Before the pandemic, most of the companies stocks were doing relatively well with Apple and Microsoft taking the lead and Pfizer trailing behind.
  2. 2020: On the onset of the pandemic around Spring, there was a fall in stock prices for all the companies, but afterwards the technology companies like Amazon, Apple, Microsoft and Google started to grow again. But companies like Pfizer, Ford and S&P 500 did not do very well especially Ford.
  3. 2021: As the vaccine rollout began and the lockdown began to be lifted, there was significant growth in the stock prices of Ford in particular given its very stock prices which was low in 2020 due to the pandemic. Companies like Google and Microsoft,S&P 500 also grew. Overall there was an improvement in the stock prices of all the companies we considered.

### Acknowledgment
Many thanks to Udacity for giving me an opportunity to try out real world problems and referencing the [Machine Learning for Trading course](https://www.udacity.com/course/machine-learning-for-trading--ud501) that gave me some insights into trading and also the help from the mentors. Thanks to the Data Scientists who have inspired and provided insights to me through Github and StackOverflow.

This project was completed as part of the [Udacity Data Scientist Nanodegree](https://www.udacity.com/course/data-scientist-nanodegree--nd025) program.
