# Trader Performance vs. Bitcoin Market Sentiment

Exploratory analysis of the relationship between Hyperliquid trader performance and the Bitcoin Fear \& Greed Index, completed as a Round-0 data science assignment.

## Contents

* `trader\_sentiment\_analysis.ipynb` — full reproducible analysis (data cleaning, merging, EDA, charts)
* `Trader\_Sentiment\_Analysis\_Report.docx` — written report with charts, tables, and strategic takeaways

## Data

Raw datasets are not included in this repo due to file size. They can be downloaded from the original sources provided in the assignment:

* Historical Trader Data (Hyperliquid): [https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing](https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing)

Bitcoin Fear \& Greed Index:[ https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc\_-mnrYv\_nhSf/view?usp=sharing](https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing)To reproduce: download both CSVs into the repo root as `historical\_data.csv` and `fear\_greed\_index.csv`, then run the notebook top to bottom.

## Key Findings

* **Profitability tracks sentiment**: average PnL per trade and win rate both peak in Extreme Greed (\~$130/trade, \~89% win rate) and are weakest in Extreme Fear/Neutral (\~$71/trade, \~76-82% win rate).
* **Traders are contrarian, not sentiment-following**: they open \~62-69% long positions during Fear, and flip to \~55-58% short during Greed — fading the crowd, and this posture coincided with stronger outcomes.
* **Capital sizing is misaligned with the edge**: average trade size is largest during Fear (\~$7.8K) and smallest during Extreme Greed (\~$3.1K) — the inverse of the regime that historically performed best.
* **Performance is concentrated**: 3 of 32 accounts generated \~46% of total realized PnL, so aggregate patterns are influenced by a small number of large/skilled traders rather than being uniform across the population.

See the full report for methodology, risk-adjusted return analysis, and strategic implications.

