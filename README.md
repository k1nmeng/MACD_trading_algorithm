# MACD_trading_algorithm

This project is a Python-based tool for analyzing stock price data and generating trading signals based on the Moving Average Convergence Divergence (MACD) indicator. It processes historical stock data from a CSV file, calculates MACD values, identifies buy and sell signals based on crossovers, and visualizes the results on an interactive candlestick chart.

!

#### 📈 Features
Data Processing: Loads and prepares time-series stock data from a standard CSV file.

MACD Calculation: Automatically calculates the MACD line, signal line, and histogram using the pandas-ta library.

Signal Generation: Implements a classic MACD crossover strategy to pinpoint potential buy (bullish) and sell (bearish) signals.

Interactive Visualization: Generates a dynamic and interactive candlestick chart using Plotly, clearly marking each buy and sell signal for easy analysis.

Exportable Chart: Saves the final chart as a standalone HTML file, perfect for sharing and analysis without needing to run any code.

#### 🛠️ How It Works
The algorithm operates on the MACD crossover strategy:

MACD Line vs. Signal Line: The core of the strategy is the relationship between the MACD line (the difference between the 12-period and 26-period EMAs) and the signal line (a 9-period EMA of the MACD line).

Buy Signal (Golden Cross): A buy signal is generated on the exact day the MACD line crosses above the signal line. This suggests a potential shift to a bullish momentum.

Sell Signal (Death Cross): A sell signal is generated on the exact day the MACD line crosses below the signal line. This suggests a potential shift to a bearish momentum.

The script scans the historical data to find every instance of these two conditions and marks them on the chart.
