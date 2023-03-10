# CryptoClustering

Instructions
1. Rename the Crypto_Clustering_starter_code.ipynb file as Crypto_Clustering.ipynb.

2. Load the crypto_market_data.csv into a DataFrame.

3. Get the summary statistics and plot the data to see what the data looks like before proceeding.

## Prepare the Data
* Use the StandardScaler() module from scikit-learn to normalize the data from the CSV file.

* Create a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

## Instructions
* Rename the Crypto_Clustering_starter_code.ipynb file as Crypto_Clustering.ipynb.

* Load the crypto_market_data.csv into a DataFrame.

* Get the summary statistics and plot the data to see what the data looks like before proceeding.

Prepare the Data
* Use the StandardScaler() module from scikit-learn to normalize the data from the CSV file.

* Create a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

## Find the Best Value for k Using the PCA Data
Use the elbow method on the PCA data to find the best value for k using the following steps:

* Create a list with the number of k-values from 1 to 11.
* Create an empty list to store the inertia values.
* Create a for loop to compute the inertia with each possible value of k.
* Create a dictionary with the data to plot the Elbow curve.
* Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.
## Answer the following question in your notebook:
1. What is the best value for k when using the PCA data? 
- When using the PCA data, the best value for 'k' is 4 because after 4, the inertia decreases and becomes linear.
2. Does it differ from the best k value found using the original data? 
- This does not differ from the k value found using the original data analysis.

## Cluster Cryptocurrencies with K-means Using the PCA Data
Use the following steps to cluster the cryptocurrencies for the best value for k on the PCA data:

* Initialize the K-means model with the best value for k.
* Fit the K-means model using the PCA data.
* Predict the clusters to group the cryptocurrencies using the PCA data.
* Create a copy of the DataFrame with the PCA data and add a new column to store the predicted clusters.
* Create a scatter plot using hvPlot as follows:
* Set the x-axis as "price_change_percentage_24h" and the y-axis as "price_change_percentage_7d".
* Color the graph points with the labels found using K-means.
* Add the "coin_id" column in the hover_cols parameter to identify the cryptocurrency represented by each data point.
## Answer the following question:
1. What is the impact of using fewer features to cluster the data using K-Means? 
- We can conclude that we can use fewer features and get a similar performance to the original model since we can clearly identify the clusters.
