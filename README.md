# Big-Data-Analytics-Project
Enhanced Stock Price Forecasting Using ARIMA, SARIMA, LSTM, and Ensemble Methods

## Time Series Analysis using ARIMA, SARIMA, and LSTM
This project focuses on analyzing and forecasting stock prices using three different models: ARIMA, SARIMA, and LSTM. The data used for this project comes from historical stock prices of Apple Inc. (AAPL).

## Project Structure
- Data Preparation and EDA:

The dataset is loaded and explored to understand its structure. We check for duplicate dates and missing values.
The columns include Date, Open, High, Low, Close, Adj Close, and Volume. The analysis focuses on the Open price.
The Date column is converted to a datetime format and set as the index for further analysis.

- Exploratory Data Analysis (EDA):

Line charts, histograms, and box plots are used to visualize the Open price and volume trends over time.
The data is split into training (data until 2020) and testing (data from 2021 onwards).

- ARIMA Model:

The Augmented Dickey-Fuller (ADF) test is used to check the stationarity of the data. The data is differenced to make it stationary if needed.
auto_arima is used to determine the best order of ARIMA parameters, and the ARIMA model is trained.
Forecasting is performed, and the results are plotted alongside the actual test data. Performance metrics like MSE, RMSE, and R-squared are computed.

- SARIMA Model:

Similar to the ARIMA model, SARIMA extends ARIMA by incorporating seasonality.
The SARIMA model is trained, predictions are made, and performance metrics are calculated.

- LSTM Model:

Data is scaled using MinMaxScaler, and time-series data is prepared for LSTM.
An LSTM model is built using Keras, and the data is split into sequences for training.
The LSTM model is trained, and the predictions are made on the test data.
Performance metrics and visualizations are used to compare the LSTM predictions with the actual values.

## Results
- Performance Metrics:
The Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared values are used to evaluate the performance of each model.
The project demonstrates the effectiveness of each model and compares their predictive abilities.

## Libraries Used
Data Manipulation and Visualization: pandas, numpy, matplotlib, seaborn
Statistical Analysis: statsmodels, pmdarima
Machine Learning: sklearn, keras, tensorflow


## Conclusion
This project illustrates the use of traditional time series models (ARIMA and SARIMA) and deep learning models (LSTM) for stock price forecasting. Each model has its strengths and weaknesses, and the results vary based on the complexity of the data and the underlying patterns.


## Architectural diagram illustrating the workflow of project:

![Screenshot 2024-11-03 112505](https://github.com/user-attachments/assets/d88f920c-e24e-495b-9de1-6fb7cf5c0901)


