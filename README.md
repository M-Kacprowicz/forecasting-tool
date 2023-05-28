# Forecasting tool

This is a project made to graduate from Gdańsk University with master's degree.

Master's thesis: Construction of a forecasting tool for forecasting stock levels based on the sales data using the Python programming language.

AutoARIMA model only accepts univariate time series, loop took around 30 minutes.

N-BEATS modle accepts multivariate time series, but I didn't have a possibility to use GPU. It was necessary to use a loop for each product, so it took around 11.5 hours.