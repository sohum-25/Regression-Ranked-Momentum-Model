# Momentum-investing using linear regression


## Strategy rules:
* Lookback 60 trading days and calculate the angle of regression and r squared value.
* Multiply the two, and rank stocks accordingly.
* Remove stocks that have moved 15% in the last 60 trading days.
* Remove stocks that are below their 100 day ema
* Check if market is above its 200 day ema
* Take top 30 stocks and make a portfolio
* Do this biweekly (approx 10 trading days)

> The strategy includes two variations in one of them we take positions regardless of the market position and in the other we check for bullishness using the 200 day ema indicator.

> The dataset is Daily prices of NIFTY 500 Stocks from 2012-1-1 to 2023-5-26 but we remove the top 10% winners to deal with survivorship bias to an extent.




