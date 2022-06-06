# improvedStratBacktest_v2 - Work In Progress

Improved + cleaner implementation of USDZAR currency L-S strategy

Older version: https://github.com/yeCodes/currencyStratBacktest

## What the project does?
This program backtests a long-short currency strategy that trades the USDZAR.

The trading signal is based on the 15-day historical moving average of USDZAR price. The portfolio goes long returns when the current price is above the 15-day MA and goes short returns when it is below.

The program sizes the position using 90-day historical vol of returns (see AHL's video on volatility scaling for more info: https://www.youtube.com/watch?v=ZJXsoZprTn8)

It also computes some important properties that characterise the strategy:
  - Sharpe ratio
  - Max drawdown period
  - Max drawdown
