![alt text](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRMjnVPxQ1YqYaAebhfADo1Dg7qhW9JiORdaHAK5MkRmC9gbqdGq-uA0GOByp3jMzGW5Wo&usqp=CAU "Baccarat")
# Baccarat
A python machine learning model that predicts stock prices and a backtesting engine to measure and estimate accuracy.

# Prerequisites
The model has only been trained with predictors of time streamed data. It has no other predictors, data points or outside factors added to the calculation.

According to the backtest, this model has a calculated accuracy of `56.9%` (backtested from 1990-2023). Not too bad, considering it out-performs the market by not using external data.

# Backtest
The project has a backtest engine. If you want to train this model with more parameters and predictors, and backtest it, you can use
```python
predictions = backtest(sp500, model, new_predictors)
```
(change new_predictors with your own predictors, or however you like).

After you have backtested your model, you can check the accuracy of your model with
```python
precision_score(predictions["Target"], predictions["Predictions"])
```

## Packages
To use the project, please install:
  - Jupyter Lab
  - Python 3.8+
  - `yfinance`, `pandas`, and `scikit-learn`.

## Data
The model has been trained with S&P500 price data, spanning from 1990-1-1 to 2023-04-12.

## Download
You can download the code for the project [here](https://github.com/Reddblue/Baccarat/blob/main/Baccarat.ipynb "Download")
