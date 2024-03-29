# Forecasting tool

This is a project made to graduate from Gdańsk University with master's degree.

Master's thesis: Construction of a forecasting tool for forecasting stock levels based on the sales data using the Python programming language.

AutoARIMA model only accepts univariate time series, loop took around 30 minutes.

N-BEATS model accepts multivariate time series, but I didn't have a possibility to use GPU. It was necessary to use a loop for each product, so it took around 11.5 hours.

Prophet model accepts only univariate time series, same as AutoARIMA model, but it can also include country holidays. Loop took around 12 minutes and is very similar to AutoARIMA loop, so it is around 3 times faster including saving csv file after each prediction made.

After processing of MAE results, it might be said that the AutoARIMA model was the best for almost every product in dataset, but Prophet model isn't much worse then AutoARIMA. Difference between results of both models are very tight. I suppose that N-BEATS model might be much better when used with GPU and maybe not generic architecture.