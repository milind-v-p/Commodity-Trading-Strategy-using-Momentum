
# Commodity Trading Strategy using Momentum

## Overview

This Python script implements a commodity trading strategy using a moving average crossover on Gold Futures (`GC=F`) with the S&P 500 index (`SPY`) as a benchmark. It calculates performance metrics including **Alpha**, **Beta**, **Sharpe Ratio**, and **Annualized Return**.

## Requirements

Install the required libraries:

```bash
pip install pandas numpy matplotlib yfinance
```

## Code Overview

1. **Data Retrieval**: Gold Futures and S&P 500 data are fetched using `yfinance`.
2. **Moving Averages**: 25-day and 50-day simple moving averages (SMA) are calculated.
3. **Trading Signals**: Buy when the short-term SMA crosses above the long-term SMA, and sell when it crosses below.
4. **Performance Metrics**: 
   - **Alpha**: Measures the strategy’s return above the benchmark.
   - **Beta**: Measures the strategy’s volatility relative to the benchmark.
   - **Sharpe Ratio**: Evaluates risk-adjusted returns.
   - **Annualized Return**: Returns adjusted for the number of trading days in a year.

## Results

The script prints the following:

- **Annualized Total Strategy Return**
- **Sharpe Ratio**
- **Alpha**
- **Beta**

It also generates a plot of Gold Futures price with the SMAs and buy/sell signals.

## Conclusion

This strategy can be adapted to other commodities or assets by changing the `symbol`. Adjust the moving average windows or benchmark to fit different market conditions.
