# Exchange Rate Time-Series Analysis using SARIMAX models

## Motivation

The foreign Exchange rates between two currencies determine the trade relations with the two countries. It includes imports and exports, tourism, foreign investments, and other internal factors like inflation and interest rates. This makes the analysis and forecasting of Exchange Rate a valuable source of insight for the economists and businesses across the globe.

## Objective

In this project, we analyzed, modeled, and forecasted exchange rate ratios of US Dollars with five other currencies - `Euro (EUR)`, `UK Pound (GBP)`, `Indian Rupees (INR)`, `Chinese Yuan (CHY)`, and `Japanese Yen (JPY)`. We used `ARIMA`, `SARIMA`, and `SARIMAX` models, and compared the accuracies of each model to determine the most reliable one. We also created an interactive MS Power Bi Dashboard that shows the time-series - historical and forecasted - to analyze the information visually.

## Data Sources

 We employed the FRED API for Python to gather live data from the FRED open-source database.

 
1. Organization for Economic Co-operation and Development, Balance of Payments BPM6: Current Account Balance: Total Balance as Percent of GDP for United States [USAB6BLTT02STSAQ], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/USAB6BLTT02STSAQ, March 27, 2024.

2. Organization for Economic Co-operation and Development, Consumer Price Index: All Items: Total for India [INDCPIALLMINMEI], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/INDCPIALLMINMEI, March 27, 2024

3. Organization for Economic Co-operation and Development, Interest Rates: Long-Term Government Bond Yields: 10-Year: Main (Including Benchmark) for India [INDIRLTLT01STM], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/INDIRLTLT01STM, March 31, 2024

4. Organization for Economic Co-operation and Development, Balance of Payments BPM6: Current Account Balance: Total Balance as Percent of GDP for India [INDB6BLTT02STSAQ], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/INDB6BLTT02STSAQ, April 5, 2024

5. U.S. Bureau of Labor Statistics, Consumer Price Index for All Urban Consumers: All Items in U.S. City Average [CPIAUCSL], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/CPIAUCSL, March 27, 2024

6. Board of Governors of the Federal Reserve System (US), Federal Funds Effective Rate [FEDFUNDS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/FEDFUNDS, April 1, 2024

7. Board of Governors of the Federal Reserve System (US), Indian Rupees to U.S. Dollar Spot Exchange Rate [EXINUS], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/EXINUS, April 2, 2024

## Data Cleaning and Pre-processing

The dataset from FRED API is clean without any missing values. The pre-processing of the datasets involved stationarizing the non-stationary data.

We did the following methods to make the datasets stationary - 

1. Seasonal Decomposition
2. Differencing

The datasets were confirmed to stationary using teh following methods - 

1. Augmented Dickey-Fuller Test
2. Auto-correlation and Partially Auto-correlation Function
3. Rolling Mean and Standard Deviation

