# Meme Stock Analysis

## Hypothesis
  * Reddit Stock screener would predict what stocks would be good to trade (long, short, options) for a period of 2 days.
  * Models would predict what were the best indicators to use.
  * List of most confident to least confident next day trading recommendations
      * Based on strength and number of indicators backing up the decision. 
      * Provide risk vs expected return thresholds for recommendations based on Sortino (greater than 1.4 is good, less than 0.9 is bad). 

  * Goal: Create a trading algo for mid / large cap stocks implementing ML and sentiment analysis.


## Key Findings
  * ARIMA model more accurately predicted stock price compared to SVM 
  * Big need for filtering on stop words for Reddit Comments!
  * Bollinger Bands: Many instances where the stock was more overbought than oversold - typical of “hype” stocks 
      * People will buy into hype
  * McGinley Dynamic MA is superior at identifying quick and slow momentum in markets
      * Ultimately not suitable for predicting good entry and exit points for meme stocks


## Conclusion
  * Extracted Data from Alpaca
      * Created Indicators 
  * Extracted posts from reddit 
      * Sentiment Analysis 
      * Most popular posts
  * Used indicators in both models to determine price action
  * ARIMA model more accurately predicted stock price compared to SVM 
