# Cryptocurrency Clustering with Unsupervised Learning

## Background

In this challenge, I utilized Python and unsupervised learning techniques to predict if cryptocurrencies are affected by 24-hour or 7-day price changes. The goal was to develop a visualization tool that would help in understanding the relationships between different cryptocurrencies based on their price changes.

## Part 1: Data Preparation

1. **Loading and Summary Statistics:**
   - Loaded the dataset `crypto_market_data.csv` into a DataFrame.
   - Obtained summary statistics and plotted the data to understand its distribution.

2. **Data Normalization:**
   - Utilized the `StandardScaler()` module from scikit-learn to normalize the data.
   - Created a DataFrame with the scaled data, setting the "coin_id" index as the index for the new DataFrame.

## Part 2: Finding the Best Value for k

1. **Using Original Scaled Data:**
   - Employed the elbow method to find the best value for k.
   - Clustered the cryptocurrencies using K-means based on the best value for k (4).

2. **Using Principal Component Analysis (PCA) Data:**
   - Performed PCA on the original scaled data to reduce features to three principal components.
   - Used the elbow method on the PCA data to find the best value for k (4).
   - Clustered the cryptocurrencies using K-means based on the best value for k with PCA data.
