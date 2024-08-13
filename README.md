#Stock Price Prediction Using RNN-LSTM

Introduction
The goal of this project is to predict future stock prices using an LSTM model, which is well-suited for time series prediction due to its ability to remember long-term dependencies in sequential data.

Dataset
The dataset used contains historical stock price data with the following features:

Date: The date of the trading session.
Open: The price at which the stock opened.
High: The highest price during the session.
Low: The lowest price during the session.
Close: The price at which the stock closed.
Adj Close: The adjusted closing price, considering dividends and stock splits.
Volume: The number of shares traded

Data Preparation
We use the adjusted closing price (Adj Close) as the feature for training the model. The dataset is preprocessed by scaling and then splitting into sequences of 60 days of data to predict the price on the 61st day.

Requirements
To run this project, you'll need the following libraries:

Python 3.x
NumPy
Pandas
Matplotlib
Scikit-learn
TensorFlow

Input and Output
Input: Sequences of 60 consecutive adjusted closing prices.
Output: Predicted price for the next day.
