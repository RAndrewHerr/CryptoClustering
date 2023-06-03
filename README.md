<img width="1000" alt="Screen Shot 2023-06-03 at 5 12 56 PM" src="https://github.com/therahgithub/CryptoClustering/assets/119986667/8705e83a-8bd1-4d7e-b620-540b9db08d65">

# CryptoClustering

In this challenge, Python and unsupervised learning were used to predict the affect of 24-hour or 7-day price changes on cryptocurrencies.

## Requirements

Find the Best Value for k by Using the Original Data
*	Code the elbow method algorithm to find the best value for k. Use a range from 1 to 11.
*	To visually identify the optimal value for k, plot a line chart of all the inertia values computed with the different values of k.
*	Answer the following question: What’s the best value for k?

<img width="1000" alt="Screen Shot 2023-06-03 at 5 45 10 PM" src="https://github.com/therahgithub/CryptoClustering/assets/119986667/7e69cd53-1933-4a2e-a5ad-bd2feaeb6e53">
  
Cluster the Cryptocurrencies with K-Means by Using the Original Data
*	Initialize the K-means model with four clusters by using the best value for k.
*	Fit the K-means model by using the original data.
*	Predict the clusters for grouping the cryptocurrencies by using the original data. Review the resulting array of cluster values.
*	Create a copy of the original data, and then add a new column of the predicted clusters.
*	Using hvPlot, create a scatter plot by setting x="price_change_percentage_24h" and y="price_change_percentage_7d". Color the graph points with the labels that you found by using K-means. Then add the crypto name to the hover_cols parameter to identify the cryptocurrency that each data point represents.

<img width="1000" alt="Screen Shot 2023-06-03 at 6 02 43 PM" src="https://github.com/therahgithub/CryptoClustering/assets/119986667/707a501d-22ec-40c1-9a5b-045ce0f575d1">
  
Optimize the Clusters with Principal Component Analysis
*	Create a PCA model instance, and set n_components=3.
*	Use the PCA model to reduce the features to three principal components. Then review the first five rows of the DataFrame.
*	Get the explained variance to determine how much information can be attributed to each principal component.
*	Answer the following question: What’s the total explained variance of the three principal components?
*	Create a new DataFrame with the PCA data. Be sure to set the coin_id index from the original DataFrame as the index for the new DataFrame. Review the resulting DataFrame.

<img width="1000" alt="Screen Shot 2023-06-03 at 5 39 29 PM" src="https://github.com/therahgithub/CryptoClustering/assets/119986667/adfed520-a705-44fe-8c9c-527f29339e38">
  
Find the Best Value for k by Using the PCA Data
*	Code the elbow method algorithm, and use the PCA data to find the best value for k. Use a range from 1 to 11.
*	To visually identify the optimal value for k, plot a line chart of all the inertia values computed with the different values of k.
*	Answer the following questions: What’s the best value for k when using the PCA data? Does it differ from the best value for k that you found by using the original data?

<img width="1000" alt="Screen Shot 2023-06-03 at 5 46 54 PM" src="https://github.com/therahgithub/CryptoClustering/assets/119986667/21e01a5b-716c-4b6d-89e7-cf1020c8a313">
  
Cluster the Cryptocurrencies with K-means by Using the PCA Data
*	Initialize the K-means model with four clusters by using the best value for k.
* Fit the K-means model by using the PCA data.
*	Predict the clusters for grouping the cryptocurrencies by using the PCA data. Review the resulting array of cluster values.
*	Create a copy of the DataFrame with the PCA data, and then add a new column to store the predicted clusters.
*	Using hvPlot, create a scatter plot by setting x="PC1" and y="PC2". Color the graph points with the labels that you found by using K-means. Then add the crypto name to the hover_cols parameter to identify the cryptocurrency that each data point represents.

<img width="1000" alt="Screen Shot 2023-06-03 at 6 03 47 PM" src="https://github.com/therahgithub/CryptoClustering/assets/119986667/e19455b2-8845-4311-98f3-50484ac532cb">

Visualize and Compare the Results
*	Create a composite plot by using hvPlot and the plus sign (+) operator to compare the elbow curve that you created from the original data with the one that you created from the PCA data.
*	Create a composite plot by using hvPlot and the plus (+) operator to compare the cryptocurrency clusters that resulted from using the original data with those that resulted from the PCA data.
*	Answer the following question: Based on visually analyzing the cluster analysis results, what’s the impact of using fewer features to cluster the data by using K-means?

<img width="983" alt="Screen Shot 2023-06-03 at 6 05 24 PM" src="https://github.com/therahgithub/CryptoClustering/assets/119986667/26ccbae0-daa6-461c-a473-97548826f76c">

<img width="984" alt="Screen Shot 2023-06-03 at 6 06 02 PM" src="https://github.com/therahgithub/CryptoClustering/assets/119986667/5892c4be-ab8c-498c-9609-b88dd3f19afa">
