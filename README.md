# ds_diksha_ballav
Trader behavior vs market sentiment analysis using Hyperliquid trading data and the Bitcoin Fear &amp; Greed Index.
# Trader Behavior vs Market Sentiment Analysis
##  Project Overview

This repository analyzes the relationship between trader behavior on the Hyperliquid platform
and overall Bitcoin market sentiment (Fear vs Greed). The objective is to evaluate how
profitability, trading activity, risk exposure, and directional bias vary under different
sentiment regimes.

## Datasets Used

1. **Bitcoin Fear & Greed Index**
   - Columns: Date, Classification (Fear / Greed)

2. **Historical Trader Data (Hyperliquid)**
   - Columns include account, symbol, execution price, size, side, leverage, closed PnL,
     timestamps, and trade metadata.

## Methodology

- Converted all timestamps to daily granularity
- Aligned both datasets by date
- Aggregated trader-level daily metrics
- Compared performance and behavior across Fear and Greed regimes
- Segmented traders based on activity frequency and PnL consistency

##  Key Metrics Analyzed

- Daily closed PnL per trader
- Win rate
- Number of trades per day
- Average trade size (USD)
- Long/short bias (buy ratio)

## Key Insights

- Trader performance (PnL and win rate) is higher during Fear periods than Greed periods.
- Trade frequency increases significantly during Fear, while Greed shows stronger long bias.
- Consistent and high-frequency traders outperform across sentiment regimes.
  
## Repository Structure

ds_diksha_ballav/
├── notebook_1.ipynb
├── csv_files/
│   └── daily_trader_metrics.csv
├── outputs/
│   ├── avg_pnl_fear_vs_greed.png
│   ├── trade_frequency_by_sentiment.png
│   └── buy_ratio_by_sentiment.png
├── ds_report.pdf
└── README.md

##  How to Run

1. Open `notebook_1.ipynb` in Google Colab  
2. Ensure notebook access is set to **Anyone with the link can view**  
3. Run all cells sequentially
   
## Notes

- All analysis was performed in Google Colab.
- This repository mirrors the exact structure required in the assignment instructions.
- Visual outputs used in the `ds_report.pdf` are stored in the `outputs/` directory.

