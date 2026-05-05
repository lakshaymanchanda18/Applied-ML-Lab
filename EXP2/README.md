# EXP 2 - Housing Price Prediction

## Overview
This experiment focuses on building a regression model to predict housing prices based on property features such as location, area, number of bedrooms, bathrooms, balcony, parking, age, and furnishing status.

## Problem Statement
Develop a regression model that can estimate the price of a house using its features. The dataset contains 120 housing records with both numerical and categorical attributes.

## Dataset Description
The dataset used in this experiment is:

- `Exp2_Housing_Price_Dataset_120_Records.csv`

### Features
- `HouseID` - Unique house identifier
- `Location` - Location category (`Urban`, `Suburban`, `Rural`)
- `Area_sqft` - Area of the house in square feet
- `Bedrooms` - Number of bedrooms
- `Bathrooms` - Number of bathrooms
- `Balcony` - Number of balconies
- `Parking` - Number of parking spaces
- `Age_Years` - Age of the house in years
- `Furnished` - Furnishing status (`Yes` / `No`)
- `Price` - Target variable representing house price

## Workflow
1. Load the dataset
2. Explore and understand the data
3. Encode categorical features
4. Split the data into training and testing sets
5. Train a regression model
6. Make predictions on test data
7. Evaluate the model using:
   - Mean Squared Error (MSE)
   - R² Score

## Libraries Used
- `pandas`
- `matplotlib`
- `scikit-learn`

## Model Used
A regression model is used to predict house prices from the input features.

## How to Run
1. Open the notebook `Experiment_2.ipynb`
2. Ensure the dataset file is available in the same folder
3. Run all cells sequentially

## Expected Outcome
The model should learn the relationship between housing features and price, and produce predictions with reasonable evaluation scores.

## Conclusion
This experiment demonstrates how regression can be applied to real-world housing data for price prediction.
