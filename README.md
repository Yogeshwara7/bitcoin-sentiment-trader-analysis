# Bitcoin Sentiment Trader Analysis

This project explores the relationship between Bitcoin market sentiment (Fear & Greed Index) and trader performance using Hyperliquid historical trading data.

## Project Overview

- **Goal:** Uncover how market sentiment influences trader behavior and profitability, and derive actionable insights for smarter trading strategies.
- **Datasets Used:**
  - **Bitcoin Fear & Greed Index:** Daily sentiment classification (Extreme Fear, Fear, Neutral, Greed, Extreme Greed).
  - **Hyperliquid Historical Trader Data:** Individual trade records with account, symbol, execution price, size, side, time, closed PnL, leverage, etc.

## Key Steps

1. **Data Loading and Cleaning:**  
   Loaded and inspected both datasets, ensuring all relevant columns are present.

2. **Data Merging:**  
   Converted timestamps to dates and merged datasets so each trade is tagged with the corresponding sentiment.

3. **Exploratory Data Analysis:**  
   - Analyzed trader performance (mean, median, std of Closed PnL) by sentiment class.
   - Examined buy vs sell behavior under different sentiment conditions.
   - Visualized average PnL by sentiment and over time.

4. **Statistical Insights:**  
   - Found that Extreme Greed periods are linked to the highest average PnL, while Neutral and Extreme Fear are lowest.
   - Observed that Sell trades outperform in Extreme Greed, while Buy trades do better in Fear.
   - Correlation between sentiment value and individual trade PnL is weak, but categorical sentiment classes show clear behavioral patterns.

5. **Time Series Analysis:**  
   - Plotted average PnL and sentiment value over time, revealing that sentiment spikes often align with changes in trader profitability.

6. **Conclusion:**  
   - Trader behavior and profitability vary with market sentiment.
   - Sentiment-aware and contrarian strategies may enhance trading outcomes.
   - See the PDF report for a detailed discussion and actionable recommendations.

## How to Run

1. Clone this repository:
git clone https://github.com/yogeshwara7/bitcoin-sentiment-trader-analysis.git

cd bitcoin-sentiment-trader-analysis

3. Install dependencies:
pip install -r requirements.txt

4. Open and run the analysis notebook:
jupyter notebook analysis.ipynb

or view the PDF report directly.

## Files

- `analysis.ipynb` — Main Jupyter notebook with code and visualizations.
- `BitcoinSentimentTraderAnalysis.pdf` — PDF report with detailed conclusions.
- `requirements.txt` — Python dependencies.
- `README.md` — Project overview and instructions.
- `images/` — (Optional) Folder for plots and figures.

## Author

- [Yogeshwara B]  
- [yogeshwara567@gmail.com]

## License

This project is for educational and demonstration purposes.

---

**Good luck with your submission! If you need a more tailored README or further help, just ask.**
