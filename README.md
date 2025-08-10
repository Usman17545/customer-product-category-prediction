# E-Commerce Customer Segmentation & Product Category Prediction

## Project Overview

This project analyzes an e-commerce customer dataset (~30,000 rows) to perform:

- Data cleaning & preprocessing
- Feature engineering & selection
- Product category prediction using machine learning
- Customer clustering for segmentation

## Dataset

The dataset contains approximately 30,000 customer records with features such as:

- Customer demographics (Age, Gender)
- Purchase behavior (Total Purchases, Amount, Total Amount)
- Product information (Product Category, Product Brand)
- Customer feedback and ratings

## Data Cleaning & Preprocessing

- Removed null and missing values to ensure data quality.
- Used boxplots to identify outliers.
- Capped outliers by increasing values below Q1 to Q1 and decreasing values above Q3 to Q3, reducing their impact while preserving data integrity.
- Encoded categorical variables:
  - Label encoding for ordinal features
  - One-hot encoding for nominal features
  - Frequency encoding for high-cardinality features (e.g., 318 unique product values)
- Scaled numerical features such as Amount and Total Amount.

## Feature Selection

- Applied SelectKBest to select the most relevant features for modeling.

## Machine Learning Model

- Built a classification model to predict product categories using selected features.
- Used Random Forest classifier.
- Evaluated the model using classification metrics: accuracy, precision, recall, and F1-score.

## Customer Clustering

- Performed K-Means clustering based on Amount, Total Amount, and Total Purchases.
- Segmented customers into groups like high spenders, moderate buyers, and low spenders.
- Visualized clusters with dimensionality reduction techniques like PCA.

