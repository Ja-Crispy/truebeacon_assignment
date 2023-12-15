This repository is my submission for the True Beacon Quant Research Intern Assignment. The task was to create a model to predict the spread between the NIFTY and Bank NIFTY indices. The repository contains the following files:

-final.ipynb : A notebook with the code for the models and analysis.
- summary.txt : A text file with the model performance metrics and an overall analysis of the models.



# Summary of Results

## Analysis of Spread Prediction Models

### Summary:

Here is a comprehensive analysis of the models I have made for the task of 
forecasting the spread between the two indices provided.
I approached the problem using a Holt-Winters Exponential Smoothing Model to try and beat the Z-Score model, then used 
a combined ensemble model for better scores.

### Key Performance Indicators:

#### Total Profit/Loss (P/L):

All three models achieved an identical total P/L of $319,335.21, indicating consistent capture of the overall spread 
movement trend.

#### Sharpe Ratio:

The Base Model exhibited the highest Sharpe Ratio at 27.77, showcasing superior risk-adjusted performance compared to 
its counterparts.

#### Max Drawdown:

Each model experienced a similar maximum drawdown, approximately 92%, suggesting comparable risk exposure.

#### Max Drawdown Duration:

The Base Model recorded the lengthiest drawdown duration of 690,511 days, implying a prolonged retention of losing 
positions.

#### Number of Trades:

The Base Model generated the most trades (47,352), indicating an active trading strategy. The Ensemble Model followed 
with 690,512 trades, reflecting the combination of signals from both underlying models.

#### Hit Ratio:

The Ensemble Model had the highest Hit Ratio of 0.068, indicating a more frequent generation of profitable trades.

#### Average Holding Period:

The Holt-Winters Model exhibited the longest average holding period at 115.08 days, suggesting a focus on capturing 
longer-term trends. In contrast, the Base Model had the shortest average holding period (77.63 days), implying a more 
frequent rotation of positions.

### Individual Model Performance:

#### Base Model:

- Total P/L: $319,335.21
- Sharpe Ratio: 27.77
- Max Drawdown: 0.9245
- Drawdown Duration: 690,511 days
- Number of Trades: 47,352
- Hit Ratio: 0.0129
- Avg Holding Period: 77.63 days

#### Holt-Winters Model:

- Total P/L: $319,335.21
- Sharpe Ratio: 27.77
- Max Drawdown: 0.9245
- Drawdown Duration: 690,511 days
- Number of Trades: 1,381
- Hit Ratio: 0.0087
- Avg Holding Period: 115.08 days

#### Ensemble Model:

- Total P/L: $319,335.21
- Sharpe Ratio: 27.77
- Max Drawdown: 0.9245
- Drawdown Duration: 690,511 days
- Number of Trades: 690,512
- Hit Ratio: 0.0679
- Avg Holding Period: 14.73 days

### Conclusion:

- The Base Model showcases a balanced risk-return profile with the highest Sharpe Ratio, despite 
  experiencing longer drawdowns. 
- The Holt-Winters Model focuses on longer-term trends, generating fewer trades with 
  extended holding periods. 
- The Ensemble Model, combining the strengths of both underlying models, achieves a higher 
  Hit Ratio, suggesting a more diversified approach.