# Time-Series-Forecast-Medium-Daily-Posts-Forecast

# Topic 

In this notebook I started with a simple dataset containing timestamps and urls of Medium publications, converted the dataset into a times series and put as a goal forecasting the number of publications per day. At the begining, I started with baseline model called Simple Exponentional Smoothing which assume that the data has no trend and no seasonality, the results were very naive and unsatisfactory. I then moved to another ETS model which is more complex in that it accounts for the trend of the data and it is applied additively, the results weren't as bad as ESE but were still unsatisfying. At the third attempt, I used the Holt Winter's seasonal Model which accounts for both the seasonality and trend and allows us to add these terms either additively or multiplicatively, this model performed the best compared with the other ETS models. In my last attempt I used the Seasonal ARIMA model, which is more complex and has Autoregressive, Integrated and Moving average terms which I determined with the help of the Autocorrelation function plot and Partial Autocorrelation function plot. Whereas for ETS models terms, I determined the terms with the help of the decomposition plot.

Finally after fiiting the models, making forecasts and ploting those forecasts for visual analysis, I have determined that Seasonal ARIMA model is the best one for this time series.


# Models

- Simple Exponential Smoothing
- Holt's Linear Method
- Holt Winter's Seasonal method
- Seasonal ARIMA

# Evaluation Metrics

- Akaike Information Criterion 
- Root Mean Squared Error
- Mean Absolute Error

# Libraries
- Numpy
- Pandas
- Matplotlib
- Statsmodels
- Scipy
- Sklearn

# Data Source

https://www.kaggle.com/code/pradneshlachake/time-series-analysis-ets-arima-sarima-prophet/data?select=medium_posts.csv
