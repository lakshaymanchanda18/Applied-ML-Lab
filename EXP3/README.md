# EXP 3 - Stock Price Prediction

## Overview
This experiment focuses on predicting stock prices using time series data and regression techniques. The goal is to forecast stock prices based on historical market information such as open, high, low, close, and volume values.

## Problem Statement
Develop a time series prediction model to forecast stock prices using historical stock data. The model should learn patterns from past records and estimate future prices.

## Dataset Description
The dataset used in this experiment contains daily stock market data with the following columns:

- `Date` - Date of the stock record
- `Stock` - Stock name or symbol
- `Open` - Opening price
- `High` - Highest price of the day
- `Low` - Lowest price of the day
- `Close` - Closing price
- `Volume` - Trading volume
- `Price` - Target value used for prediction

## Workflow
1. Load the stock dataset
2. Understand the data structure
3. Preprocess and encode required features
4. Split the data into training and testing sets
5. Train a regression model
6. Make predictions
7. Evaluate the model using:
   - Mean Squared Error (MSE)
   - R² Score

## Libraries Used
- `pandas`
- `pickle`
- `scikit-learn`

## Model Used
A `LinearRegression` model is used for predicting stock prices from historical data.

## How to Run
1. Open the notebook `Experiment_3.ipynb`
2. Make sure the dataset file is available in the correct path
3. Run all notebook cells sequentially
4. Check the output metrics and predictions

## Expected Outcome
The trained model should be able to identify trends in stock data and generate reasonable price predictions.

## Conclusion
This experiment demonstrates how regression and time series data can be used to forecast stock prices.
