# MLTrader - Automated Trading Strategy using Machine Learning Sentiment Analysis

This readme file contains the whole description and the process of working of the project 
The execution is as follows - 

1. Install miniconda or anaconda from the internet
2. Setup and install anaconda
3. Create your alpaca account
4. Generate your API key and secret from Alpaca 
5. Enter your key and secret into the code 
6. Run the program
7. The current status of the trades will be dispayed 
8. After finishing graphs for the trades will be automatically generated

## Introduction
MLTrader is an automated trading strategy implemented in Python, leveraging machine learning sentiment analysis to make buy or sell decisions in the stock market. It utilizes the Alpaca trading API for executing trades and Yahoo Finance data for backtesting.

## Features
- **Sentiment Analysis**: Utilizes machine learning sentiment analysis to gauge market sentiment based on news headlines.
- **Position Sizing**: Dynamically adjusts position size based on available cash and risk tolerance.
- **Bracket Orders**: Places bracket orders with take-profit and stop-loss levels for risk management.
- **Backtesting**: Conducts backtesting using historical stock market data to evaluate the performance of the strategy.

## Prerequisites
- Python 3.x
- Required Python packages: `lumibot`, `alpaca_trade_api`, `finbert_utils`, `timedelta`


## Configuration
1. Obtain Alpaca API credentials from [Alpaca Markets](https://alpaca.markets/).
2. Replace `API_KEY` and `API_SECRET` in `mltrader.py` with your Alpaca API credentials.
3. Set `PAPER` to `True` if you are using the Alpaca paper trading environment.

## Usage
1. Modify `mltrader.py` to adjust parameters such as the target symbol and cash at risk.
2. Run the strategy:
    ```
    python mltrader.py
    ```

## Backtesting
1. Define the start and end dates for backtesting in `mltrader.py`.
2. Run the backtest:
    ```
    strategy.backtest(YahooDataBacktesting, start_date, end_date, parameters={"symbol":"AAPL", "cash_at_risk":0.5})
    ```

## Disclaimer
This project is for educational purposes only and does not constitute financial advice. Use it at your own risk.

