# Data-Science-Regression-Project-Predicting-Home-Prices-in-Bangalore
This project is a Python-based solution for predicting house prices in Bangalore. It leverages machine learning and data analysis techniques to provide accurate price estimates based on various parameters.

## Code Overview
The code is organized into different sections, each of which performs specific tasks. Here's a brief overview of what each section does:

## Data Loading and Initial Exploration
- Imports necessary libraries and configures the matplotlib settings.
- Loads the dataset from 'Bengaluru_House_Data.csv' using Pandas.
- Displays the first few rows of the dataset.
- Shows the shape of the dataset.
- Group the data by 'area_type' and aggregates the counts. 

## Data Preprocessing
- Removes unnecessary columns ('area_type', 'society', 'balcony', 'availability').
- Handles missing values by dropping rows with missing values.
- Extracts the number of bedrooms ('bhk') from the 'size' column.
- Converts non-numeric values in 'total_sqft' to a numeric representation.
- Calculates the price per square foot.
- Handles location data by categorizing locations with very few data points as 'other.'

## Outlier Detection and Removal

- Identifies and removes outliers in the 'price_per_sqft' column.
- Defines functions for scatter plots and outlier removal based on the number of bedrooms.
- Removes outliers based on the number of bedrooms.

## Data Visualization
- Generates a histogram of 'price_per_sqft.'
- Displays unique values in the 'bath' column.
- Identifies and removes rows with an unusually high number of bathrooms.

## Model Building
- Prepares the data for machine learning by encoding categorical features.
- Splits the dataset into features (X) and the target variable (y).
- Splits the data into training and testing sets.
- Builds a Linear Regression model and evaluates its performance using cross-validation.

## Hyperparameter Tuning
- Uses GridSearchCV to find the best model among Linear Regression, Lasso, and Decision Tree Regression.

## Price Prediction Function
- Defines a function to predict house prices based on location, square footage, number of bathrooms, and number of bedrooms.

# Usage 
You can use the trained model to predict house prices by providing the required input parameters (location, square footage, number of bathrooms, and number of bedrooms). Please refer to the code for an example of how to use the prediction function.

# Model and Data

The code uses a Linear Regression model for price prediction, and the data is based on the 'Bengaluru House Data' dataset provided in the code.

Feel free to explore the code further and customize it to fit your specific needs. Enjoy predicting house prices in Bangalore!









