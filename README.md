# ML_CryptoClustering_Unsupervise
With the use of Python and unsupervised learning, to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.


![yPredict-thumbnail-3](https://github.com/T800-101A/ML_CryptoClustering_Unsupervise/assets/122810519/8cfaf52e-444f-4523-bd04-80af9bad8947)


Find the Best Value for k by Using the Original Data :

    Code the elbow method algorithm to find the best value for k. Use a range from 1 to 11. 
    
    To visually identify the optimal value for k, plot a line chart of all the inertia values computed with the different values of k.
    
    Answer the following question: What’s the best value for k? 

    ![Screenshot from 2023-11-14 03-04-05](https://github.com/T800-101A/ML_CryptoClustering_Unsupervise/assets/122810519/e0234470-5815-4901-9b74-0c5989cbc287)



Cluster the Cryptocurrencies with K-Means by Using the Original Data :

    Initialize the K-means model with four clusters by using the best value for k. 
    
    Fit the K-means model by using the original data. 
    
    Predict the clusters for grouping the cryptocurrencies by using the original data. Review the resulting array of cluster values.
    
    Create a copy of the original data, and then add a new column of the predicted clusters. 
    
    Using hvPlot, create a scatter plot by setting x="price_change_percentage_24h" and y="price_change_percentage_7d". Color the graph points with the labels that you found by using K-means. Then add the crypto name to the hover_cols parameter to identify the cryptocurrency that each data point represents. 

    ![Screenshot from 2023-11-14 03-05-24](https://github.com/T800-101A/ML_CryptoClustering_Unsupervise/assets/122810519/30c2e3f9-3c26-47fb-b0ce-3c66b92fa7b9)



Optimize the Clusters with Principal Component Analysis :

    Create a PCA model instance, and set n_components=3. 
    
    Use the PCA model to reduce the features to three principal components. Then review the first five rows of the DataFrame.
    
    Get the explained variance to determine how much information can be attributed to each principal component. 
    
    Answer the following question: What’s the total explained variance of the three principal components?
    
    Create a new DataFrame with the PCA data. Be sure to set the coin_id index from the original DataFrame as the index for the new DataFrame. Review the resulting DataFrame. 
    
    ![Screenshot from 2023-11-14 03-06-52](https://github.com/T800-101A/ML_CryptoClustering_Unsupervise/assets/122810519/90e7b7bf-c556-4778-b607-2fd6551cf7b6)
    ![Screenshot from 2023-11-14 03-07-58](https://github.com/T800-101A/ML_CryptoClustering_Unsupervise/assets/122810519/ad905a28-08da-4511-9e01-9f4a971f20c5)

    


## Find the Best Value for k by Using the PCA Data :

    Code the elbow method algorithm, and use the PCA data to find the best value for k. Use a range from 1 to 11. 
    
    To visually identify the optimal value for k, plot a line chart of all the inertia values computed with the different values of k. 
    
    Answer the following questions: What’s the best value for k when using the PCA data? Does it differ from the best value for k that you found by using the original data? 
   
    ![Screenshot from 2023-11-14 03-09-03](https://github.com/T800-101A/ML_CryptoClustering_Unsupervise/assets/122810519/6d986c4f-827e-430f-bfdc-d7aebba24cd4)


## Cluster the Cryptocurrencies with K-means by Using the PCA Data :

    Initialize the K-means model with four clusters by using the best value for k. 
    
    Fit the K-means model by using the PCA data.
    
    Predict the clusters for grouping the cryptocurrencies by using the PCA data. Review the resulting array of cluster values.
    
    Create a copy of the DataFrame with the PCA data, and then add a new column to store the predicted clusters.
    Using hvPlot, create a scatter plot by setting x="PC1" and y="PC2". Color the graph points with the labels that you found by using K-means. Then add the crypto name to the hover_cols parameter to identify the cryptocurrency that each data point represents. 
    ![Screenshot from 2023-11-14 03-09-47](https://github.com/T800-101A/ML_CryptoClustering_Unsupervise/assets/122810519/4f2026d5-49aa-4bb6-80b3-bba481fdc730)


## Visualize and Compare the Results
    To receive all points, you must:
    
    Create a composite plot by using hvPlot and the plus sign (+) operator to compare the elbow curve that you created from the original data with the one that you created from the PCA data. 
    ![Screenshot from 2023-11-14 03-10-43](https://github.com/T800-101A/ML_CryptoClustering_Unsupervise/assets/122810519/acb5e4c6-f9c8-423f-816d-17b12712451b)

    Create a composite plot by using hvPlot and the plus (+) operator to compare the cryptocurrency clusters that resulted from using the original data with those that resulted from the PCA data. 
    
    Answer the following question: Based on visually analyzing the cluster analysis results, what’s the impact of using fewer features to cluster the data by using K-means? 




