Pairs Trading Analysis

Overview

This project performs a pairs trading analysis using historical data for selected stocks across different markets. Pairs trading is a market-neutral trading strategy that involves identifying two correlated stocks, monitoring their price movements, and executing trades when there’s a deviation in their relationship.

Objectives

The primary objectives of this project are:

	•	To identify pairs of stocks with strong historical correlations.
	•	To conduct statistical tests to validate the chosen pairs.
	•	To develop and backtest a trading strategy that capitalizes on temporary price divergences between paired stocks.

Stocks and Markets Analyzed

The analysis includes stock pairs from multiple sectors and markets, specifically focusing on:

	•	Market 1: [Market name, e.g., U.S. Technology Sector]
	•	Stock Pair: [Example - Apple (AAPL) and Microsoft (MSFT)]
	•	Market 2: [Market name, e.g., European Utilities Sector]
	•	Stock Pair: [Example - EDF and E.ON]
	•	Market 3: [Market name, e.g., Asian Financial Sector]
	•	Stock Pair: [Example - Mitsubishi UFJ Financial (MUFG) and Mizuho Financial (MFG)]

(Replace these with the actual markets and stocks from your analysis)

Methodology

	1.	Data Collection
	•	Historical price data is collected for the selected pairs over a specified period.
	•	Data sources include publicly available financial APIs or datasets.
	2.	Correlation and Cointegration Testing
	•	The stock pairs are evaluated for correlation and cointegration to ensure a stable, long-term relationship.
	•	Key statistical tests include the Augmented Dickey-Fuller (ADF) test and Johansen cointegration test.
	3.	Trading Strategy
	•	A pairs trading strategy is implemented where trades are executed based on the spread between the paired stocks.
	•	When the spread deviates from its mean by a threshold amount, positions are opened expecting a reversion to the mean.
	•	Both entry and exit points are calculated based on z-scores of the spread.
	4.	Backtesting
	•	The strategy is backtested over historical data to assess profitability and risk.
	•	Key metrics evaluated include Sharpe ratio, maximum drawdown, and win/loss ratio.

Results

	•	The notebook generates visualizations of price movements, spread, and trading signals.
	•	Performance metrics provide insights into the effectiveness of the pairs trading strategy over the backtest period.

Dependencies

	•	Python libraries: pandas, numpy, matplotlib, statsmodels, and yfinance (if applicable).
	•	Ensure all dependencies are installed before running the notebook.

Usage

	1.	Clone the repository and navigate to the project directory.
	2.	Run the Jupyter Notebook to view the analysis and results:

jupyter notebook EQT_Pairs_trading_graphs.ipynb


	3.	Modify stock tickers and parameters within the notebook to analyze different pairs or markets.

Conclusion

This project demonstrates a market-neutral approach to trading based on statistical relationships between stock pairs. While pairs trading can mitigate directional market risk, real-time execution and transaction costs are essential factors for practical implementation.
