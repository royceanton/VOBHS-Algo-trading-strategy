# VOBHS-Algo-trading-strategy
An implementation and backtest analysis of VOBHS algorithmic trading strategy using NumPy, Pandas and Backtesting using Backtesting.py

# What is VOBHS Indicator

VOBHS Technical Strategy that analyzes the volume and current market trend to filter buy and sell signals algorithmically. The strategy comprises of the following indicators:

```
Volatility-Oscillator

Boom-Hunter Pro (Pinescript to Python implementation)

Hull-Moving Average

Modified Average True range for Stop Loss
```
# Analysis and Backtest

> [VOBHS Strategy implementation](https://github.com/royceanton/VOBHS-Algo-trading-strategy/blob/main/vobhs-single-asset.ipynb)

> [VOBHS Strategy backtest using Backtesting.py](https://github.com/royceanton/VOBHS-Algo-trading-strategy/blob/main/vobhs-backtest.ipynb)

# Technical Indicators Implemented

### Volatility Oscillator

![image](https://i.gyazo.com/aede35dcd46f562cc7c70ade8e8184ec.png)

Price movement follows a regular and consistent pattern where it will gradually decline before accelerating and bottoming out. Similar to how the price will frequently increase gradually before accelerating into a peak.

No matter the type of market being traded or the trading strategy being employed, it is important to distinguish between moderate, steady price movements and more extreme, accelerated price movements. These accelerated price movements are related to exceptional market circumstances, which call for a trader to be alert and organized. A Volatility Oscillator can also take advantage of accelerated price movements by giving additional confirmation on actual trend happening on market.

**Study on Volatility Oscillator**

> [Volatitlity Oscillator Study & Visualisation](https://jovian.ai/ranton95/volatility-oscillator-1)

### Boom-Hunter Pro (Veryfid)

![image](https://i.gyazo.com/f58555df01b47cbb979d51563a2bdbd8.png)

The original Boom-pro indicator by [Veryfid](https://wiki.boomhunter.net/) in pinescript language reverse engineered and implemented on Python. 

Note: Only certain segments of the complete Boom indicator modified for VOBHS strategy has been implemented here.

**Study on Boom Hunter Pro**
> [Boom-Pro Indicator Analysis](https://jovian.ai/ranton95/boom-hunter-pro)

### Hull Moving Average (HMA)

![Image](https://i.gyazo.com/ac826a3c8d2efd43b6a46d345bdfea8b.png)

The Hull Moving Average (HMA) seeks to maintain the smoothness of the moving average line while reducing the lag of a conventional moving average. This indicator, created by Alan Hull in 2005, prioritizes more recent values and significantly reduces lag by using weighted moving averages.

**Study on Hull MA**
> [Hull MA Analysis & Visualisation](https://jovian.ai/ranton95/hull-ma-1)



# VOBHS Strategy Backtest result
![image](https://i.gyazo.com/45c939e9df46218622c4434ddde662bc.png)

```
Start                                     0.0
End                                    1499.0
Duration                               1499.0
Exposure Time [%]                        31.4
Equity Final [$]                   10131.9031
Equity Peak [$]                    10131.9031
Return [%]                           1.319031
Buy & Hold Return [%]                0.952299
Return (Ann.) [%]                         0.0
Volatility (Ann.) [%]                     NaN
Sharpe Ratio                              NaN
Sortino Ratio                             NaN
Calmar Ratio                              0.0
Max. Drawdown [%]                   -2.007586
Avg. Drawdown [%]                   -1.720264
Max. Drawdown Duration                  317.0
Avg. Drawdown Duration                  234.5
# Trades                                  1.0
Win Rate [%]                            100.0
Best Trade [%]                       1.446258
Worst Trade [%]                      1.446258
Avg. Trade [%]                       1.446258
Max. Trade Duration                     470.0
Avg. Trade Duration                     470.0
Profit Factor                             NaN
Expectancy [%]                       1.446258
SQN                                       NaN
_strategy                      Vobhs_Strategy
_equity_curve                       Equity...
_trades                      Size  EntryBa...
dtype: object
```
