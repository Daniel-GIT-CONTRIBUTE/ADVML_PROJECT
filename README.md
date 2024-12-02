
# COMPARING XGBOOST, GAM, MVGAM, PROPHET, AND LSTM ON THE S&P500
A project for COMP 6936

# Dependencies
### Dependencies (main file "predictor_project.ipynb):  
  - Jupyter Lab, Jupyter Notebook, Google Colab, or any program that reads .ipynb file
  - numpy, pandas, pygam, sklearn, matplotlib, plotly, xgboost, tensorflow.keras, Prophet (facebook), yfinance
### Additional Dependencies (sub file "mvgam.ipynb):  
  - the language R, mvgam, dplyr, marginaleffects, ggplot2, patchwork
    
# How to run:
  - view the compiled project here in GITHUB
  - OR use a .ipynb software like Google Colab or Jupyter
  - OR run the .py file but the dependent libraries must all be installed

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
  - Test 
  - 

  # Sites Consulted:
     1. Nicholas Clarck, "MVGAM", https://ecogambler.netlify.app/blog/autocorrelated-gams/
     2. Gregg Hogg, "Stock Price Prediction & Forecasting with LSTM Neural Networks in Python", https://www.youtube.com/watch?v=CbTU92pbDKw&t=1537s
     3. OWCZAR, "GAM Model for Time-Series Forecasting", https://www.kaggle.com/code/owczar/gam-model-for-time-series-forecasting

  
    
