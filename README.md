# twitter-data-analysis-4

This repo focuses on how to do tfidf on Japanese language. 

# Update on cleaning Japanese Tweets

We can see the word metrics is not that beautiful, so let's adjust the parameters of tfidf to make it easy to read. 

# Update on adding stopwords list

I added more words to the stopwords list. Now the clusters are prettier.  
Next, I will use some visualization tools to show the result. 

# Update on using elbow method to find the right K

In this repo, I applied elbow method to find the right amount of K for the K-means.  

The math behind this method is that for every K, you calculate the total Sum of Squared Errors (SSE). 
Then we plot the chart of SSE in relation to K. 

The point where SSE start to decrease slowly is the elbow point. 

When k==4, we notice an elbow point. 
Therefore, we set the K==4. 

# Update on some explanation on K means clustering algorithm

K means clustering algorithm is an unsupervised machine learning technique used to cluster data. 

Unspervised machine learning means the cases where you don't know your target variable or class. Instead, we 
try to identify the underlying structure in the data. 

1. Start with K centroids by putting them at random place. 

2. Compute distance of every point from centroid and cluster them accordingly. 

3. Adjust centroids so that they become center of gravity for given cluster. 

4. Re-cluster every point based on their distance with centroid. 

5. Again adjust centroids.

6. Recomputer clusters and repeat this till data points stop changing clusters. 
