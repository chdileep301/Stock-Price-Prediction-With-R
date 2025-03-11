Overview:
This project forecasts stock prices using time series models like ARIMA, Exponential Smoothing, Naive, Seasonal Naive, and Neural Networks.
It fetches stock data from Yahoo Finance, analyzes it, and provides visualizations and forecasts.

Data Acquisition and Storage:
The script uses the quantmod package to fetch stock data from Yahoo Finance via its API.
Data is cached locally in a CSV file for future use, stored in the data folder.
The script checks if the data already exists in the CSV file; if not, it fetches fresh data and saves it.

Models Used:
ARIMA: Auto-regressive Integrated Moving Average for time series forecasting.
Exponential Smoothing: Smooths past data to predict future values.
Naive Model: Uses the last observed value as the forecast.
Seasonal Naive Model: Similar to Naive but accounts for seasonality.
Neural Network: Uses a neural network for non-linear forecasting.

Shiny Dashboard:
The project includes a Shiny dashboard for interactive visualization of forecasts and model diagnostics.
The dashboard displays residual diagnostics, ACF/PACF plots, and Ljung-Box test results for model evaluation.

How to Use:
Clone the repo and run stock_forecast.r.
Modify the symbol and predict_months variables to analyze different stocks and forecast periods.
The script will fetch data, apply models, and generate forecasts with accuracy metrics
