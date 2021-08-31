# S-P-500-Hourly-Prediction-and-Investiment-Model

## Abstract 
Using stock market data, we planned to create a pool investment vehicle which could help users manage their assets by investing the stock market. To accomplish our goals, we implemented two different models: Light GBM Regressor, and SGD Regressor. We conducted a real world simulation with 5 million dollars as a base fund, and found Light GBM Regressor could outperform SGD Regressor with a promising 12% yearly return. 

## Introduction
With the increasing mainstream use of high frequency trade and price prediction on the stock market, our team proposed an alternative angle at benefitting from trading using Machine Learning to predict and optimize for investment combinations hourly. 

We are trying to create a pool investment vehicle[1], which uses funds from many numerous individual investors. Based on our models’ prediction of all ~500[2] stocks’ future value, we invest all the funds evenly (i.e. the same amount of money is invested in each stock) throughout the S&P 500, with long and short positions. 

For our transaction, it’s not trading based on the highest and lowest price during the hour, it is based on the beginning of the hour and the prediction of our model for the end of this hour, which we extract from financial intraday data. Financial stock data commonly consists of Open, High, Low, Close, and other features. For our model, we are only taking advantage of “O” and “C” instead of “H” and “L” or other features, which means we are not trying to make the most profit out of the transaction hour, but to make sure that we can make a safe profit. The intuition is, as long as we predict the correct direction trend for a stock, as long as it outperforms the transaction fee, we’ll have made a profit. 

##Dataset
The main dataset ( a 10-year range S&P hourly price data for 300+ tickers) is too big to include so I uploaded it onto my personal server, feel free to download. 
url: http://songyunxiao.live/static/files/S&P-10-year-range-hourly-data.rar

