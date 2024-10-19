# BTC Candlestick Analysis

## Introduction
This project is focused on analyzing Bitcoin price data using candlestick patterns and various technical indicators such as RSI (Relative Strength Index) and MACD (Moving Average Convergence Divergence). By utilizing historical price data, the project aims to predict future price trends and provide valuable insights for traders.

## Features
- **Candlestick Analysis**: Extracts Open, High, Low, and Close (OHLC) values of Bitcoin price for candlestick charting.
- **Technical Indicators**: Calculates RSI and MACD indicators to enhance the analysis.
- **Predictive Modeling**: Uses a deep learning model (LSTM) to predict future candlestick patterns for up to 30 days.
- **Visualization**: Visualizes the predicted candlestick data using the `mplfinance` library, showing key price movements.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/BTC-Candlestick-Analysis.git
   ```
2. Install the necessary dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Download Bitcoin data for the desired period:
   ```python
   btc_data = yf.download('BTC-USD', period='1y', interval='1d')
   ```
2. Run the model to predict future candlestick patterns:
   ```bash
   python main.py
   ```
3. Visualize the predicted candlestick chart for the next 30 days.

## Example Output
The project provides a candlestick chart showing predicted Open, High, Low, and Close values for Bitcoin prices, along with key technical indicators. Example output:
```
Day 1: Open: 30000, High: 31000, Low: 29000, Close: 30500
...
Day 30: Open: 32000, High: 32500, Low: 31500, Close: 32200
```

## Model
The deep learning model utilizes an LSTM (Long Short-Term Memory) network to analyze and predict future candlestick patterns. The model is trained on historical Bitcoin data and fine-tuned to predict prices for the next 30 days.


