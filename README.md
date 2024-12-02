
# COMPARING XGBOOST, GAM, MVGAM, PROPHET, AND LSTM ON THE S&P500
A project for COMP 6936

# Dependencies (main file "predictor_project.ipynb):  
  - Jupyter Lab, Jupyter Notebook, Google Colab, or any program that reads .ipynb file
  - numpy, pandas, pygam, sklearn, matplotlib, plotly, xgboost, tensorflow.keras, Prophet (facebook), yfinance
# Additional Dependencies (sub file "mvgam.ipynb):  
  - the language R, mvgam, dplyr, marginaleffects, ggplot2, patchwork
    
# How to run:
  - view the compiled project here in GITHUB
  - OR use a .ipynb software like Google Colab or Jupyter
  - OR run the .py file but the dependent libraries must all be installed

# Data  
## Data used:
  - source: S&P500
  - description: the index of the fortune 500 companies in the USA
## Data split:
  - train: Jan 1, 1980 - Dec 31, 2020 
  - test: Jan 1, 2021 - Current
## Predictors for train:
  - Quarter
  - Year
  - Month
  - Day of week
  - Yesterday's Close Price
## Predictors for test:
  - Quarter
  - Year
  - Month
  - Day of week


# ML Methods:
  - Models: XGBoost, GAMs, LSTM, Facebook Prophet, MVGAM 
  - Scores: RMSE (residual means squared error)

# There are 13 variables (X) and 1 output of zero or one(y)
  - The 13 variables in order are:
    - 0.age
    - 1.sex
    - 2.chest pain type (4 values)
    - 3.resting blood pressure
    - 4.serum cholestoral in mg/dl
    - 5.fasting blood sugar > 120 mg/dl
    - 6.resting electrocardiographic results (values 0,1,2)
    - 7.maximum heart rate achieved
    - 8.exercise induced angina
    - 9.oldpeak = ST depression induced by exercise relative to rest
    - 10.the slope of the peak exercise ST segment
    - 11.number of major vessels (0-3) colored by flourosopy
    - 12.thal: 0 = normal; 1 = fixed defect; 2 = reversable defect
    - **The names and social security numbers of the patients were recently removed from the database, replaced with dummy values.

  # Sites Consulted:
    - https://www.geeksforgeeks.org/generalized-additive-model-in-python/
    - https://pygam.readthedocs.io/en/latest/notebooks/tour_of_pygam.html
  
    
