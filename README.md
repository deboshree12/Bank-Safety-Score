# Overview
This project analyzes the stock prices of major US banks - JP Morgan Chase, Bank of America, Wells Fargo, Citigroup, and Goldman Sachs - from January 2000 to December 2022, along with the corresponding US GDP data. The project aims to forecast the monthly returns for each bank and calculate safety scores based on the forecasted returns.

# Libraries Used
The project uses the following libraries:

- `yfinance` for downloading the historical stock price data for the banks
- `pandas` for data manipulation and analysis
- `numpy` for numerical calculations and data manipulation
- `matplotlib and seaborn` for data visualization
- `fredapi` for downloading US GDP data
- `statsmodels` for time series analysis and modeling
- `sklearn` for calculating mean absolute error

# Steps
The following are the main steps of the project:

- Download historical stock price data for the banks using the yfinance library.
- Download US GDP data using the fredapi library and merge it with the bank stock price data.
- Fill missing values in the data using forward fill and backward fill.
- Check for and remove outliers using the IQR method.
- Plot the time series data for the major banks and GDP to visualize trends and patterns.
- Calculate the correlation matrix and visualize it using a heatmap to identify relationships between the variables.
- Calculate monthly returns for the data and split it into training and testing sets.
- Normalize the data using mean and standard deviation.
- Create and fit a VAR model to the training data.
- Forecast the future returns using the VAR model.
- Calculate safety scores based on the forecasted returns for each bank.
- Calculate the Mean Absolute Error (MAE) for each bank to measure the accuracy of the model.
- Visualize the actual vs. predicted stock prices for each bank to compare and analyze the results.
- Visualize the safety scores as a bar plot to compare and analyze the results.

# Results
The project successfully forecasts the monthly returns for each bank using the VAR model and calculates safety scores based on the forecasted returns. The safety scores indicate the banks' safety based on their future stock price movements. The MAE scores provide a measure of the accuracy of the model's predictions. The safety score bar plot provides a clear visualization of the safety scores for each bank.

<img width="1003" alt="Screenshot 2023-03-21 at 4 59 22 PM" src="https://user-images.githubusercontent.com/49270107/227018651-68eb82de-348a-4107-8237-bdecffabb95f.png">


Overall, the project successfully analyzed the stock prices of major banks and GDP data from the US, and used this data to predict future returns and calculate safety scores. The results showed that the model was more accurate in predicting the returns of some banks compared to others, and that some banks were safer investments than others based on their safety scores.
