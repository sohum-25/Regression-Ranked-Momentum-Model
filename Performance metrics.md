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



# Metrics 

Both the strategies look like they outperform the market but the strategy with the bullish market filter tends to outperform the one without the filter.
>A chunk of data has to be left out initially for the calculation of all the necessary values for the portfolio simulation, hence the first trade is from 2013-08-20 to 2023-05-19 which is approximately 9.7 years.
![image](https://github.com/sohum-25/Momentum-investing/assets/37628069/957b7b1d-2ec5-4ff4-9a53-80e2df3719fd)

| Strategy          | Returns | CAGR |
|-------------------|-----------|------| 
| Regression Strategy with 200ema filter  | 442.98% | 16.49%|
| Regression Strategy          | 237.02% | 9.25% |
| Market            | 205.99% | 7.69% |

There seems too be a much more significant difference when we come to the Drawdowns
Both the strategies have a lower drawdown as compared to the market, but there is significantly lower downside to the strategy with the filter.

![image](https://github.com/sohum-25/Momentum-investing/assets/37628069/d1b58b50-3d7f-49b0-98a6-f18369881581)



| Strategy          | Drawdowns |
|-------------------|-----------|
| Regression Strategy with 200ema filter  | -26.84% |
| Regression Strategy          | -52.29% |
| Market            | -64.54% |
