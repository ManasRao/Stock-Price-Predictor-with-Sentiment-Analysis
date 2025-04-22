# Stock Price Prediction Using News Sentiment (LSTM)

This project explores how sentiment from daily financial news headlines can be used to improve stock price prediction using an LSTM (Long Short-Term Memory) model. By combining sentiment analysis with historical stock data, the model aims to capture market behavior influenced by real-world events.

---

## How to Run

1. **Scrape News Headlines**  
   Run `news_scrapping.ipynb` to collect daily news headlines.

2. **Perform Sentiment Analysis**  
   Use `sentiment_analysis.ipynb` to compute sentiment scores (positive, negative, neutral, compound) for each headline.

3. **Prepare the Dataset**  
   Run `data_prep.ipynb` to merge stock data with sentiment scores and format it for model input.

4. **Train the Model**  
   Open `training.ipynb` to train the LSTM model and evaluate prediction results.

---

## LSTM-Based Modeling Approach

The model is designed to capture temporal patterns in stock prices using past data sequences. It is trained on normalized feature values including historical prices and sentiment metrics. This setup helps the LSTM model learn correlations and trends over time.

---

## News Sentiment Integration

Sentiment scores are derived from daily financial headlines using natural language processing. The intuition is that political events, policy changes, and global news directly influence market performance. For example, major policy announcements or judicial verdicts have historically led to sharp price changes (e.g., CPEC or Panama Papers).

By incorporating both current and next-day headlines, the model accounts for short-term market reactions and aims to make better end-of-day price predictions.

---

## Summary of Algorithm

- Collect news headlines.
- Analyze sentiment (positive, negative, neutral, compound).
- Merge with historical stock data.
- Format data into sequences for LSTM input.
- Train the model and predict future stock prices.

---

## Output

Prediction results and visualizations can be found in `output.png`.
