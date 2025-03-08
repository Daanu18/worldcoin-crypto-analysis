# Worldcoin Crypto Analysis

## Overview

This project provides a detailed system for analyzing Worldcoin cryptocurrency prices using real-time and historical data. The system is designed to collect, process, and visualize market data, including:

- Live price data from Binance API
- Historical OHLCV (Open, High, Low, Close, Volume) data
- Trading volume analysis
- Market trends and volatility visualization
- Automated error handling for API requests

## Features

- **Real-Time Data Fetching**: Uses the `ccxt` library to fetch Worldcoin data from Binance every 15 minutes.
- **OHLCV Data Processing**: Retrieves Open, High, Low, Close, and Volume (OHLCV) data for analysis.
- **CSV Data Storage**: Saves historical data to `crypto_data.csv` and appends new data dynamically.
- **Visualization**: Uses `matplotlib` for plotting price trends and market movements.
- **Timeframe Selection**: Allows users to choose different timeframes (e.g., 15-minute intervals).
- **Rate-Limited API Requests**: Ensures API requests adhere to Binance’s rate limits to prevent restrictions.
- **Trigger Function for Automated Execution**: A function that activates when the closing price of Worldcoin exceeds a predefined threshold (e.g., $2.5), printing a message and continuing execution.
- **Error Handling & Exception Catching**: Implements a robust mechanism to catch errors and retry failed API requests.

## Graphs

The script generates the following visualizations:

- **Close Price Over Time**: A line graph showing the closing price of Worldcoin over time.
- **Volume Over Time**: A bar chart showing the trading volume of Worldcoin over time.
- **High vs Low Prices**: A line graph comparing the high and low prices of Worldcoin.
- **Close Price with Moving Average**: A line graph showing the closing price along with its 20-period moving average.

## Installation & Requirements

To run the Jupyter Notebook, ensure you have the following installed:

- Python 3.x
- Jupyter Notebook or Jupyter Lab
- Required Python libraries:
  ```bash
  pip install ccxt pandas matplotlib

## Running the Notebook

Clone this repository
- git clone https://github.com/your-username/worldcoin-crypto-analysis.git

Navigate to the repository folder
- cd worldcoin-crypto-analysis

Launch Jupyter Notebook
- jupyter notebook worldcoin.ipynb

## Potential Applications

- Market trend analysis.
- Financial forecasting and research.
- Algorithmic trading insights.
- Cryptocurrency market anomaly detection.
- Automated crypto data tracking for trading strategies.

## Contributing

If you'd like to contribute to this project, feel free to:
- Open an issue to report bugs or suggest improvements.
- Submit a pull request with your changes.
