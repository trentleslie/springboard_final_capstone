Capstone Three: LSTM Neural Network Candlestick Forecasting for Short-term Trading Opportunities
==============================

Given that stock prices can be modeled by a random walk, forecasting prices may seem to be an exercise in futility. However, using neural networks to identify patterns in OHLC data may provide some insight for potential trading opportunities. In trading, a popular approach in technical analysis is the use of candlestick patterns to identify potential reversals or continuation in price changes over time. This relies on price over time reflecting collective psychology that tends to repeat itself and the tendency for prices to regress to a longer-term mean. Further, incorporating information other than price itself, such as volume, moving averages, and RSI, may yield more reliable models in practice as traders and algorithms rely on these for making decisions. In conjunction with some trading rules, such as avoiding shorts on indices (since they tend to go up over time) and stop-loss orders based on volume profile, a model or set of models may provide an edge to grow an account over time. 

To reduce risk and maximize returns on short-term (1-5 trading days) trades, what are the expected open, high, low, and close (OHLC) prices for a given index, stock, ETF, forex, or futures contract tomorrow? What are the expected OHLC prices for the following week? What is the most effective rolling window size for training data?

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
