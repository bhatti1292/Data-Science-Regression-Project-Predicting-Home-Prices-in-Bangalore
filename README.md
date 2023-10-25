# Data-Science-Regression-Project-Predicting-Home-Prices-in-Bangalore
This project is a Python-based solution for predicting house prices in Bangalore. It leverages machine learning and data analysis techniques to provide accurate price estimates based on various parameters.

# Code Overview
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
