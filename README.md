# pandas_stocks_analysis
Analysis of Bollinger Bands, SMA, stock volume, and movement.
This project encompasses a range of stock market analysis and trading strategies leveraging various indicators and methodologies. The primary goal is to determine optimal buying and selling points for stocks, based on different financial and statistical measures.

![image](https://github.com/Tomlowe7/pandas_stocks_analysis/assets/126796950/700bdba7-b7e3-4b5e-9d65-6d3240960ce2)


### buy_sell_stocks_Bolligner_Bands
Goal: The project's objective is to utilize Bollinger Bands to signal when to buy and sell stocks. Bollinger Bands are derived from a 20-period simple moving average (SMA) plus or minus two times the 20-period rolling standard deviation. When the stock price crosses the upper band, it indicates an overbought condition, signaling a potential sell. Conversely, when the stock price crosses the lower band, it suggests an oversold condition, signaling a potential buy.
Libraries: The notebook imports libraries such as yfinance for financial data, pandas for data manipulation, and matplotlib for visualization.
Data: The notebook fetches historical data for the SPY ticker (which typically tracks the S&P 500 index) for a specific date range using the yfinance library.
Bollinger Bands Calculation: The notebook computes the upper and lower Bollinger Bands based on the stock's closing price.

### buy_sell_stocks_SMA
Goal: The objective of this project is to utilize short and long-term moving averages to visualize and interpret stock trend changes. When the stock price crosses the long-term moving average downwards, it's typically a bearish sign, suggesting a potential sell. Conversely, when the stock price crosses the long-term moving average upwards, it's generally a bullish sign, signaling a potential buy. The notebook specifically aims to generate buy and sell signals for Tesla (TSLA) stock.
Libraries: The notebook imports libraries such as numpy and pandas for data manipulation, yfinance for financial data, and plotly for visualization.
Data: The notebook fetches 5 years of historical data for the TSLA ticker using the yfinance library.
Moving Averages Calculation: The notebook computes a 30-day simple moving average (SMA) based on the stock's adjusted closing price.

### buy_sell_stocks_volume
Goal: The project's objective is to build a trading analysis system that provides signals on when to buy or sell stocks in an investment portfolio. The strategy is predominantly based on volume changes. A significant increase in trading volume is interpreted as a favorable entry point, suggesting it's an opportune time to buy.
Libraries: The notebook imports libraries like pandas, numpy, datetime, math, and warnings.
Data: The notebook loads data from CSV files: adjclose.csv (which seems to have adjusted close prices) and volume.csv (which likely contains trading volume data). It computes the percentage change in trading volume.
Simulation Setup: The notebook seems to set up a simulation starting from January 2, 2017, to October 1, 2020, with a starting capital of $1,000,000.

### predict_stocks_movement
Goal: The project's objective is to predict the likelihood of upward movement for all S&P 500 stocks. The analysis involves looping over all S&P 500 members and calculating the probability of each stock moving upward after it has moved downward for N onsecutive days (where N ranges from 1 to 10). Before each trading day, the probability of a stock moving upward is computed based on its recent downward trend. This approach is also applied to Sector ETFs.
Libraries: The notebook imports libraries like pandas, numpy, yfinance, and pandas_datareader.
Data: The notebook fetches a list of S&P 500 companies from a Wikipedia page and then downloads the adjusted close prices for these stocks using the yfinance library.

### Dependencies
pandas
numpy
yfinance
pandas_datareader
plotly
matplotlib
