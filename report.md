# Market Sentiment Analysis Report

## Methodology

The analysis combines Market Fear & Greed Index data with historical Hyperliquid trading records by aligning both datasets at the daily level. The preprocessing stage included handling missing values, removing duplicate records, converting timestamps into standardized datetime formats, and merging the datasets using the trading date.

Several behavioral metrics were engineered to characterize trader performance, including daily Closed PnL, win rate, average trade size, trade frequency, and long/short activity. Since leverage information was not present in the provided dataset, leverage-based analyses were omitted.

To evaluate whether market sentiment influenced trading outcomes, both descriptive statistics and inferential statistical tests were performed. A Welch's t-test compared average profitability between sentiment regimes, while the non-parametric Mann–Whitney U test was used because trading PnL exhibited a highly skewed distribution with many break-even trades and several large outliers.

Trader segmentation was then performed using trading frequency, average position size, and historical win rate to identify distinct behavioral groups.

---

## Key Insights

### Insight 1
Although Fear days produced a higher average Closed PnL (**54.29**) than Greed days (**42.74**), Welch's t-test did not identify a statistically significant difference in mean profitability (**t = 1.851, p = 0.064**). However, the Mann–Whitney U test indicated a highly significant difference in the distribution of trading outcomes (**p < 0.001**), suggesting that market sentiment affects trading behavior even if average profitability alone does not capture the full effect.

### Insight 2

Extreme Greed produced the highest proportion of profitable trades (**46.49%**) and the lowest proportion of break-even trades (**47.86%**), indicating that strong bullish sentiment increases the likelihood of decisive trade outcomes.

### Insight 3

Standard Fear conditions exhibited fewer losing trades (**6.13%**) than ordinary Greed conditions (**11.57%**), suggesting that traders may behave more selectively or conservatively during periods of moderate market pessimism.

---

## Strategy Recommendations

### Strategy 1 — Trade Selectively During Fear

Moderate Fear periods were associated with fewer losing trades and a higher average PnL than ordinary Greed periods. Traders may benefit from maintaining disciplined entries during Fear while avoiding excessive risk-taking during Extreme Fear.

### Strategy 2 — Capture Momentum During Extreme Greed

Extreme Greed produced the highest proportion of profitable trades. Traders may increase participation during strong bullish sentiment while employing predefined profit targets or trailing stop-loss orders to protect gains against sudden market reversals.

---

## Conclusion

This analysis demonstrates that hyperliquid market sentiment influences trader behavior more strongly than average profitability alone suggests. While differences in mean Closed PnL between Fear and Greed periods were not statistically significant, the distribution of trade outcomes varied substantially across sentiment regimes. These findings indicate that combining sentiment indicators with behavioral trading metrics can provide valuable insights for market timing, risk management, and the development of more robust quantitative trading strategies.
