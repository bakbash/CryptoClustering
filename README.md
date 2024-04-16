# CryptoClustering

## Overview

This project applies machine learning techniques to cluster cryptocurrencies based on their historical performance and characteristics. We use K-means clustering and Principal Component Analysis (PCA) to analyze and visualize the underlying patterns in the data.

## Data Preparation

### Steps
1- Normalize Data: Utilize StandardScaler() from scikit-learn to scale features for uniformity.
2- DataFrame Creation: Construct a DataFrame with scaled data and set coin_id as the index.

## Dataset Details

* Total Data Points: 77,536
* Training Set: 58,152
* Test Set: 19,384

## Clustering Analysis

### Finding the Best Value for k

* Method: Elbow method with k values from 1 to 11 to determine the optimal cluster count.
* Visualization: Plot inertia values to identify the best k.

## K-means Clustering on Scaled Data

1- Initialization: Configure K-means with the optimal k value.
2- Model Fitting: Apply the K-means model on the original scaled DataFrame.
3- Prediction: Classify cryptocurrencies and append predictions to the data.
4- Visualization: Create scatter plots with hvPlot to illustrate clusters with dimensions PC1 vs PC2.


## PCA Optimization

1- Apply PCA: Reduce feature dimensions to three principal components.
2- Variance: Analyze the explained variance to assess information retention.
3- DataFrame Creation: Generate a new DataFrame with PCA results, maintaining coin_id as the index.

## K-means on PCA Data

* Procedure: Similar to the scaled data approach but using the PCA-transformed data.
* Visualization: Adjust scatter plot axes to price_change_percentage_24h vs price_change_percentage_7d.

## Results and Insights


* Optimal k values: Analysis of both original and PCA data to determine the best clustering approach.
* Cluster Visualization: Compare clustering results from the original and PCA-reduced data.
* Impact Analysis: Discuss the effect of reducing features on the clustering outcome.

## Visualizations

* Composite Plots: Use hvPlot to create composite plots comparing different analyses.

  
