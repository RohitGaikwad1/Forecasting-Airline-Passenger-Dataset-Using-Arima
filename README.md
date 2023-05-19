# Forecasting-Airline-Passenger-Dataset-Using-Arima
This project appears to be focused on analyzing and forecasting airline passenger data using time series analysis techniques. Here is a description of the steps and methods used in the project:
Data Preparation:
The project starts by importing necessary libraries such as pandas, numpy, matplotlib, seaborn, and statsmodels.
The "Airlines+Data.xlsx" file is read into a pandas DataFrame called "airline".
The "Month" column is converted to a datetime format and set as the index of the DataFrame.
Exploratory Data Analysis:
The original passenger data is plotted over time using matplotlib.
Rolling mean and standard deviation are calculated using a window size of 12 (representing 12 months) and plotted.
Augmented Dickey-Fuller test is performed to check the stationarity of the time series data.
Data Transformation:
Log scale transformation is applied to the passenger data, and the transformed data is plotted.
Moving average of the log-transformed data is calculated, and the moving average and log-transformed data are plotted.
The difference between the log-transformed data and the moving average is computed and plotted.
Seasonal decomposition is performed on the log-transformed data to separate the trend, seasonality, and residual components.
Stationarity Testing:
The stationarity of the transformed data is checked using rolling mean and standard deviation plots.
Augmented Dickey-Fuller test is applied to the transformed data to confirm stationarity.
Autocorrelation and Partial Autocorrelation Analysis:
Autocorrelation and partial autocorrelation functions are calculated and plotted to determine the order of ARIMA models.
Building Models:
Three types of ARIMA models are built: AR (autoregressive), MA (moving average), and ARIMA (autoregressive integrated moving average).
The models are fitted to the differenced log-transformed data, and the fitted values are plotted.
The Root Mean Squared Error (RSS) is calculated to evaluate the model fit.
Forecasting:
The fitted values of the ARIMA model are used to predict future values.
The differenced predictions are then cumulatively summed to obtain the overall predictions.
The predictions are converted back to the original scale using exponential transformation.
The original passenger data and the predicted values are plotted together.
Visualization and Interpretation:
Various plots are generated to visualize the original data, fitted values, and predictions.
The plot_predict function is used to visualize the forecasted values.
Overall, this project aims to analyze the airline passenger data using time series analysis techniques, transform the data to achieve stationarity, build ARIMA models, and make predictions for future values.
