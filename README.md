# UCITS Strategy: Regularization Methods in US Equity Market

***NOTE: CODE AVAILABLE UPON REQUEST***

## Introduction 
* The goal of the strategy is to exploit the inefficiency of cap-weighted index using Regularization methods and obtain an extraperformance over the benchmark. 
* By replying a market index, you are implicitly giving a larger weight to the largest companies, but there's no empirical evidence to justify it. 
* The framework consists in identifying the most important stocks that have defined benchamark's returns using regularization methods. In this application, the number of stocks considered is 20, in order to meet UCITS diversification constraints.

## Data

The strategy is applied in US Large Cap Equity market, with the S&P 500 index selected as benchmark.
The data is collected for the period January 2005-Decmber 2020, while the backtesting period is January 2008-December 2020. 



## Results

### Summary statistics:

![summary stats](https://user-images.githubusercontent.com/78954578/130291490-4cb198d8-51dc-4c46-ae22-2dc0c3fdce0d.png)

* Over the period considered, the strategy is able to deliver greater annualized returns and risk-adjusted performance, measured by the Sharpe ratio; the annualized alpha reaches 10%.
* Drawbacks come with higher VaR, CVaR and maximum drawdown, all suggesting a deeper tail risk.
* By jointly analyzing the higher moments of the distribution, we can also observe extreme positive events, as can be easily seen by visualizing the portfolio's returns distribution:

<img width="545" alt="hist" src="https://user-images.githubusercontent.com/78954578/130271762-ffb773e2-d828-46bd-bcd3-55cc48edcdcf.png">

### Ex-post P&Ls comparison:

<img width="555" alt="montante" src="https://user-images.githubusercontent.com/78954578/130251583-e901ccbc-b72f-4090-8430-0c3e1421b949.png">

* Starting from a 1000$ capital, the cumulative profits of the strategy over 13 years (2008-2020) would have reached 12.800$, while the same amount invested in the market would have allowed to obtain a final wealth of approximately 2.500$.

### Yearly performance:

<img width="545" alt="year" src="https://user-images.githubusercontent.com/78954578/130251990-df796db4-070b-48e3-8298-f83f7ec28dd6.png">

* A desirable characteristic of an active fund is the "beat the market" ability: ideally, a manager asks for a higher management fee than a passive strategy to perform better than the market. In this case, if we define a new metric, the Hit Ratio, as the percentage number of periods a portfolio beats the benchmark, the strategy achieves a descrete performance of 61,5% (8 out of 13 years).


## Conclusions

* The strategy is able to deliver a greater Sharpe ratio, expected returns and an outstanding annualized alpha of 10% over the period 2008-2020
* The strategy seems to act like an amplifier of benchmark movements: it performs incredibly better than the benchmark when the market goes up, but this comes with a worse perfomance during bearish periods.
