Stock Market Prediction Using Machine Learning

This project aims to predict the future closing price of the S&P 500 index using machine learning techniques, specifically the Random Forest Classifier. The S&P 500 is a stock market index that measures the stock performance of 500 large companies listed on stock exchanges in the United States.

Project Overview

The project involves the following steps:

1. Data Collection: We use the yfinance library to fetch historical data of the S&P 500 index.
2. Data Preprocessing: We clean the data by removing unnecessary columns and create new columns for future predictions.
3. Feature Engineering: We create a new column called 'Target' which is set to 1 if the closing price of the next day is greater than the closing price of the current day.
4. Model Training: We use the Random Forest Classifier from the sklearn library to train our model. The model is trained on features like 'Close', 'Volume', 'Open', 'High', and 'Low'.
5. Model Evaluation: We evaluate the model using the precision score from the sklearn.metrics module.
6. Backtesting: We backtest the model by training it on a rolling window of data and testing it on the next window.
7. Feature Expansion: We create new features based on rolling averages of different horizons to improve the model's performance.

Requirements:
    1. Python 3.6 or above
    2. Libraries: yfinance, pandas, sklearn

Usage:
To use this project, clone the repository and run the Python script. Make sure you have the required libraries installed.

Limitations:
The predictions made by the model are not very accurate. This is because stock prices are influenced by a multitude of factors, many of which are not included in this model. This project is a demonstration of how machine learning can be applied to financial data and should not be used for making actual investment decisions.

Future Work:
Improvements can be made by incorporating more features into the model, such as company fundamentals, macroeconomic indicators, or sentiment analysis from news articles or social media. Additionally, other machine learning models or ensemble methods could be explored to improve prediction accuracy.