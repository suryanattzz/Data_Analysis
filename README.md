# Trading Analysis with Market Sentiment

A comprehensive analysis project exploring the relationship between trader performance and Bitcoin market sentiment using Hyperliquid historical trading data and Fear & Greed Index metrics.

## Project Overview

This project analyzes two primary datasets:

1. **Bitcoin Market Sentiment Dataset** (`fear_greed_index.csv`)
   - Columns: Date, Classification (Fear/Greed)
   - Source: Crypto Fear & Greed Index

2. **Historical Trader Data from Hyperliquid** (`historical_data.csv`)
   - Columns: account, symbol, execution price, size, side, time, start position, event, closedPnL, leverage, etc.
   - Contains trader performance metrics and execution details

## Objective

- Explore the relationship between trader performance and market sentiment
- Uncover hidden patterns in trading behavior during fear vs. greed periods
- Deliver insights that can drive smarter trading strategies

## Project Structure

```
├── Trading_analysis.ipynb          # Main Jupyter notebook with analysis
├── features_daily_acct_sym.csv     # Features aggregated by account & symbol
├── features_daily_bucket.csv       # Features aggregated by sentiment bucket
├── features_daily.csv              # Daily aggregated features
├── trades_with_sentiment.csv       # Trades matched with sentiment data
├── README.md                       # This file
```

## Data Files

- **features_daily_acct_sym.csv**: Daily features by account and coin
  - Columns: trade_date, account, coin, sentiment_bucket, trades, pnl, win_rate, notional, fg_value_mean, pnl_per_notional

- **features_daily_bucket.csv**: Daily features aggregated by sentiment bucket

- **features_daily.csv**: Daily aggregated features across all traders

- **trades_with_sentiment.csv**: Individual trades with corresponding market sentiment

## Installation & Setup

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- pandas, numpy, matplotlib, seaborn

### Install Dependencies
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Run Analysis
```bash
jupyter notebook Trading_analysis.ipynb
```

## Usage

1. Open the Jupyter notebook: `Trading_analysis.ipynb`
2. Run all cells to execute the analysis
3. Review visualizations and insights generated

## Key Insights

- Impact of market sentiment (Fear vs. Greed) on trading performance
- Win rate and PnL correlation with sentiment periods
- Account-level performance patterns during different sentiment phases
- Strategy recommendations based on sentiment analysis

## Files Generated

The analysis generates processed feature files:
- Aggregated metrics by account, symbol, and sentiment
- Time-series data for sentiment correlation analysis
- Performance statistics by trading period

## Contributing

Feel free to extend the analysis with additional metrics, visualizations, or datasets.

## License

This project is for educational and analytical purposes.

## Author

Created for trading strategy research and market sentiment analysis.

---

**Last Updated**: January 2026
