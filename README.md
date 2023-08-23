# Stock-performance-analysis

This code snippet appears to be a Python script written within a Jupyter Notebook for performing stock market data analysis. The analysis includes the following steps:

1. **Importing Libraries**: The code imports necessary libraries such as pandas for data manipulation, matplotlib for visualization, and yfinance for downloading stock data.

2. **Time Range Setup**: The script defines a time range for which stock data should be collected. It uses the current date to determine a 3-month time window.

3. **Ticker List Creation**: A list of stock ticker symbols (AAPL, MSFT, NFLX, GOOG) is defined.

4. **Data Download and Storage**: Stock data for each ticker within the specified time range is downloaded using the yfinance library and stored in a dictionary, where each ticker's data is a separate DataFrame.

5. **Data Concatenation**: The individual DataFrames for each ticker are concatenated into a single DataFrame with a multi-level index containing the tickers and dates.

6. **Data Preprocessing**: The concatenated DataFrame is reset to have a standard index structure.

7. **Visualization of Stock Performance**: The code generates line plots to visualize the stock performance for each ticker. It plots the closing prices and rolling averages (moving averages) with different window sizes. Each ticker has its own subplot.

8. **Calculation of Volatility**: The script calculates the volatility of each stock's closing prices using percentage changes and a rolling standard deviation over a 10-day window.

9. **Visualization of Volatility**: It creates line plots to visualize the volatility of each stock over time. Each stock's volatility is plotted on a separate subplot.

10. **Correlation Analysis**: The script performs correlation analysis between different stocks. Initially, it focuses on the correlation between Apple (AAPL) and Microsoft (MSFT) by creating a DataFrame containing their closing prices and then visualizing the correlation using a scatter plot.

11. **Extended Correlation Analysis**: The script further extends the correlation analysis by creating DataFrames for pairwise correlations between all combinations of tickers. It then generates scatter plots for each pair of stocks to visualize their correlations.

Overall, the code aims to provide insights into stock performance, volatility, and correlations through visualizations and data analysis. It combines data from various tickers, applies rolling averages and volatility calculations, and visually represents the results using line plots and scatter plots.
