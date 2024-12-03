
# COMPARING XGBOOST, GAM, MVGAM, PROPHET, AND LSTM ON THE S&P500
A project for COMP 6936

# Dependencies
### Dependencies (main file "predictor_project.ipynb):  
  - Jupyter Lab, Jupyter Notebook, Google Colab, or any program that reads .ipynb file
  - numpy, pandas, pygam, sklearn, matplotlib, plotly, xgboost, tensorflow.keras, Prophet (facebook), yfinance
### Additional Dependencies (sub file "mvgam.ipynb):  
  - the language R, mvgam, dplyr, marginaleffects, ggplot2, patchwork
    
# How to run:
  - view the compiled project here in GITHUB by clicking "predictor_project.ipynb" (no dependencies required)
  - OR use a .ipynb software like Google Colab or Jupyter and open "predictor_project.ipynb"


# Data  
### Data used:
  - source: S&P500
  - description: the index of the fortune 500 companies in the USA
### Data split:
  - train: Jan 1, 1980 - Dec 31, 2020 
  - test: Jan 1, 2021 - Current
### Predictors for train:
  - Quarter
  - Year
  - Month
  - Day of week
  - Yesterday's Close Price
### Predictors for test:
  - Quarter
  - Year
  - Month
  - Day of week


# ML Methods:
  - Models: XGBoost, GAMs, LSTM, Facebook Prophet, MVGAM 
  - Scores: RMSE (residual means squared error)

# ML data processing implementation
### XGBoost
  - Train Process: DF of train data
  - Test Process: custom loop where the model predicts, appends the data, then based off this, predicts again for n number of times
### GAMs
  - Train Process: DF of test data
  - Test Process: DF of train data
### LSTM
  - Train Process: custom DF with 100 lag features. So each day has Time-1 ~ Time-100 of the previous predictors 
  - Test Process:custom DF with 100 lag features, but feature "close price" is all masked to 0.
### Prophet
  - Train Process: DF of test data
  - Test Process: prophet's built-in future data generation with no features other than a single date
### MVGAM
  - Train Process: DF of test data exported to R. Lacks all features but index (simple int) and close price.
  - Test Process: DF of train data exported to R. Lacks all features but index (simple int). All close price masked as 0.

  # Sites Consulted:
     1. Nicholas Clarck, "MVGAM", https://ecogambler.netlify.app/blog/autocorrelated-gams/
     2. Gregg Hogg, "Stock Price Prediction & Forecasting with LSTM Neural Networks in Python", https://www.youtube.com/watch?v=CbTU92pbDKw&t=1537s
     3. OWCZAR, "GAM Model for Time-Series Forecasting", https://www.kaggle.com/code/owczar/gam-model-for-time-series-forecasting

  
    
