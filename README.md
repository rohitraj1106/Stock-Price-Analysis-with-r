📈 Stock Price Analysis using R

This project demonstrates basic stock price analysis techniques using R, specifically focusing on moving average analysis. We leverage the quantmod and TTR packages to retrieve stock data and analyze trends using 50-day and 200-day simple moving averages (SMA).

📌 Introduction
Stock price analysis helps investors understand market trends and make informed investment decisions. In this project, we analyze Apple Inc.'s stock data using simple yet effective technical analysis tools.

📦 Prerequisites
Make sure you have the following R packages installed:

install.packages("quantmod")
install.packages("TTR")
🧪 Steps
🔹 Step 1: Fetch Stock Data
We retrieve historical stock data for Apple Inc. (AAPL) using quantmod::getSymbols() from Yahoo Finance. The data includes:

Daily Open, High, Low, Close prices

Volume

Adjusted Close prices

🔹 Step 2: Calculate Moving Averages
We calculate:

50-day SMA: Short-term trend

200-day SMA: Long-term trend

These help smooth out fluctuations and reveal underlying trends.

🔹 Step 3: Visualize Trends
Using chartSeries() and addSMA(), we plot:

Daily stock price chart

50-day and 200-day SMAs

We also identify:

Bullish crossover: 50-day SMA crosses above 200-day → potential buy signal

Bearish crossover: 50-day SMA crosses below 200-day → potential sell signal

📊 Sample Output
Line chart showing AAPL stock prices with 50-day and 200-day SMAs

(Insert image here if applicable)

✅ Conclusion
We successfully analyzed Apple’s stock prices using moving averages. This method provides a foundation for further technical analysis. The project can be extended with advanced models such as:

ARIMA for time series forecasting

Machine learning models for price prediction

📁 Project Structure
bash
Copy
Edit
📂 stock-price-analysis/
├── stock_analysis.R      # Main R script
└── README.md             # Project overview

📎 References
>quantmod CRAN page
>Yahoo Finance
