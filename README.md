# oibsip_taskno_3

# Data Cleaning Project: New York City Airbnb Open Data

## Project Overview

This project focuses on cleaning and preparing the New York City Airbnb Open Data for analysis. Data cleaning is a crucial step in data analysis and ensures that the dataset is accurate, consistent, and ready for further exploration or modeling.

## Dataset

- **Source:** [New York City Airbnb Open Data](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)
- **Description:** This dataset contains information about Airbnb listings in New York City, including details about the host, location, price, availability, and reviews.

## Objectives

The main objectives of this project are:
1. **Ensure Data Integrity:** Verify the accuracy, consistency, and reliability of the dataset.
2. **Handle Missing Data:** Impute or manage missing values to ensure completeness.
3. **Remove Duplicates:** Identify and eliminate duplicate records to maintain data uniqueness.
4. **Standardize Data:** Ensure consistent formatting and units across the dataset.
5. **Detect and Remove Outliers:** Identify and address outliers to prevent skewed analysis.

## Steps Performed

### 1. Data Integrity Check
- Ensured that the data was consistent and accurate.
- Verified logical consistency between related columns (e.g., `minimum_nights` <= `maximum_nights`).

### 2. Missing Data Handling
- Imputed missing values using appropriate methods:
  - Mean for continuous numerical data (e.g., `price`).
  - Median for skewed numerical data (e.g., `number_of_reviews`).
  - Mode for categorical data (e.g., `room_type`).
  - Specific placeholder values for text-based columns (e.g., `'Unknown'` for `host_name`).

### 3. Duplicate Removal
- Removed duplicate records based on unique identifiers (`id`, `host_id`).

### 4. Data Standardization
- Standardized data formats and ensured consistent units.
- Adjusted column formats where necessary for analysis.

### 5. Outlier Detection and Removal
- Identified outliers in numerical columns using the Interquartile Range (IQR) method.
- Removed rows that contained outliers to ensure data quality.

## Results

- The cleaned dataset is now free of duplicates, standardized, and has no missing values.
- Outliers were removed, improving the overall reliability of the data for further analysis.

## Tools & Technologies

- **Python**: Primary programming language used.
- **Pandas**: Used for data manipulation and cleaning.
- **Google Colab**: Used for developing and documenting the project.

## Conclusion

This project demonstrates the importance of data cleaning in preparing a dataset for analysis. By ensuring data integrity, handling missing data, removing duplicates, standardizing formats, and addressing outliers, the dataset is now ready for further exploration, visualization, and modeling.
