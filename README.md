Capstone Three: LSTM Neural Network Candlestick Forecasting for Short-term Trading Opportunities
==============================

Given that stock prices can be modeled by a random walk, forecasting prices may seem to be an exercise in futility. However, using neural networks to identify patterns in OHLC data may provide some insight for potential trading opportunities. In trading, a popular approach in technical analysis is the use of candlestick patterns to identify potential reversals or continuation in price changes over time. This relies on price over time reflecting collective psychology that tends to repeat itself and the tendency for prices to regress to a longer-term mean. Further, incorporating information other than price itself, such as volume, moving averages, and RSI, may yield more reliable models in practice as traders and algorithms rely on these for making decisions. In conjunction with some trading rules, such as avoiding shorts on indices (since they tend to go up over time) and stop-loss orders based on volume profile, a model or set of models may provide an edge to grow an account over time. 

To reduce risk and maximize returns on short-term (1-5 trading days) trades, what are the expected open, high, low, and close (OHLC) prices for a given index, stock, ETF, forex, or futures contract tomorrow? What are the expected OHLC prices for the following week? What is the most effective rolling window size for training data?

Project Organization
------------

    ├── LICENSE
    ├── README.md            <- The top-level README for developers using this project.
    ├── data
    │   ├── interim          <- Intermediate data that has been transformed (broken down by ticker).
    │   ├── predict          <- Processed data for prediction (concatentated ticker data).
    │   ├── predict_tomorrow <- Final prediction output with forecast and stats.
    │   ├── processed        <- The final, canonical data sets for modeling (concatenated ticker data).
    │   └── raw              <- The original, immutable data dump from the Alpha Vantage API.
    │                           All data folders are too large for github, can be found at the link below:
    │                           https://drive.google.com/drive/folders/1GD7eRp6cpy9bNZ1-FH3uYSbgolxLo-Na?usp=sharing
    │
    ├── models               <- Trained and serialized models, model predictions, or model summaries
    │                           Too large for github, can be found at the link below:
    │                           https://drive.google.com/drive/folders/1GTdTCJE6fAOJ5NslOw--fFqh1MGkMKIn?usp=sharing
    │
    ├── notebooks            <- Jupyter notebooks. 
    │
    ├── reports            <- Generated analysis as Word documents, PDF, PowerPoint slide decks, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    └── requirements.yml   <- The requirements file for reproducing the analysis environment, can be
                              imported in Anaconda (may need to updated prefix)

--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
