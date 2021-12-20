# Time_series_Homework
Unit 10 - A Yen for the Future

## Time-Series Forecasting

This assignment looked at historical Dollar-Yen exchange rate futures data.  With this data we applied time series analysis and modeling to determine whether there was any predicable beharior.

The following modeling was used:
>Decomposting using a Hodrick-Prescott Filter

>Forecasting Returns using an ARMA Model

>Forecasting the Settle Price using ARIMA Model

>Forecasting Volatility with GARCH

Based on the above modelingthe following conclusion was reached:
While the yen price is forecasted to increase in the next 5 day the rest of the modeling would make me question the purchase.  The time series analysis results were above the 0.05 threshold so I would not rely on this analysis to purhcase the yen.  Based on the GARCH model the alpha(2) was greater than 0 which indicates that the volatility of the yen is expected to increase.  Therefore, I would not feel confident using these models for trading.

## Linear Regression Forecasting

I built a Scikit-Learn linear regression model to predict Yen futures returns with lagged yen futures returns and categorical calendar seasonal effects.

 After preparing the data, fitting a lnear regression model, making predictions using the testing data and evaluationg the out-of-sample and in-sample performance my out-of sample root mean squared error was 0.415454 and the in-sample root mean squared error was 0.5962.  Typically, an in-sample error will be lower than an out-of sample error; therefore, I wouldn't recommend using this model.