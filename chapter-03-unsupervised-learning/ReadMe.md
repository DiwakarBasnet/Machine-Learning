# Unsupervised Learning:

Unsupervised learning refers to algorithms that learn patterns from unlabeled data.
In contrast to supervised learning where models learn to map the input to the target output, unsupervised methods learn concise representations of the input data, which can be used for data exploration or to analyze or generate new data.
The algorithms used in unsupervised learning can mainly be categorized into three types, they are;<br>

## 1. Clustering:

Using clustering algorithm means we're going to give the algorithm a lot of input data with no labels and let it find any groupings in the data it can. Those groupings are called clusters. A cluster is a group of data points that are similar to each other based on their relation to surrounding data points.
Clustering is used for things like feature engineering or pattern discovery. When we're starting with data we know nothing about, clustering might be a good place to get some insight.
Types of clustering algorithm;<br>

### (i) Hierarchical clustering:

This clustering technique is further divided into two types:<br>
* **Agglomerative Hierarchical clustering** - In this technique, initially each data point is considered as an individual cluster. At each iteration, the similar clusters merge with other clusters until one cluster or K clusters are formed.<br>
* **Divisive Hierarchical clustering** - In simple words, we can say that the Divisive Hierarchical clustering is exactly the opposite of the Agglomerative Hierarchical clustering. In Divisive Hierarchical clustering, we consider all the data points as a single cluster and in each iteration, we separate the data points from the cluster which are not similar. Each data point which is separated is considered as an individual cluster. In the end, we’ll be left with n clusters.<br>

### (ii) K-Means clustering:

The K-means algorithm identifies k number of centroids, and then allocates every data point to the nearest cluster, while keeping the centroids as small as possible.
The K-means algorithm in data mining starts with a first group of randomly selected centroids, which are used as the beginning points for every cluster, and then performs iterative calculations to optimize the positions of the centroids.<br>
It halts creating and optimizing clusters when either:
* The centroids have stabilized - there is no change in their values because the clustering has been successful.
* The defined number of iterations has been achieved.

### (iii) [DBSCAN clustering](https://www.analyticsvidhya.com/blog/2020/09/how-dbscan-clustering-works/):

It stands for Density-Based Spatial Clustering of Applications with Noise. K-Means and Hierarchical Clustering both fail in creating clusters based on varying densities. That's why we need DBSCAN clustering. DBSCAN is a density-based clustering algorithm that works on the assumption that clusters are dense regions in space separated by regions of lower density.<br><br>
DBSCAN requires only two parameters: *epsilon* and *minPoints*. ***Epsilon***  is the radius of the circle to be created around each data point to check the density and ***minPoints*** is the min number of data points required inside that circle for that data point to be classified as a Core point. A data point is a **Core** point if the circle around it contains at least *'minPoints'* number of points. If the number of points is less than *minPoints*, then it is classified as **Border** point and if there is no other data points around any data point within *epsilon* radius, then it is treated as **Noise**.

### (iv) [Gaussian Mixture Models]([https://www.analyticsvidhya.com/blog/2019/10/gaussian-mixture-models-clustering/](https://towardsdatascience.com/gaussian-mixture-models-explained-6986aaf5a95)):

Gaussian Mixture Models are probabilistic models and use the soft clustering approach for distributing the points in different clusters. A Gaussian Mixture is a function that is comprised of several Gaussians, each identified by k ∈ {1,…, K}, where K is the number of clusters of our dataset. Each Gaussian k in the mixture is comprised of the following parameters:
* A mean μ that defines its centre.
* A covariance Σ that defines its width. This would be equivalent to the dimensions of an ellipsoid in a multivariate scenario.
* A mixing probability π that defines how big or small the Gaussian function will be.

## 2. Association rule learning:

It tests for the reliance of one data element on another data element and design appropriately so that it can be more cost-effective. It is employed in *Market Basket analysis*, *Web usage mining*, *continuous production*, etc. There are following types of Association rule learning;

### (i) Apriori algorithm:

This algorithm detects the most frequent itemsets or elements in a transaction database and establishes association rules between the items. This algorithm needs frequent datasets to produce associate rules. It needs a breadth-first seach and hash tree to compute the itemset efficiently. It is generally used for market basket analysis and support to learn the products that can be purchased together. It can be used in the healthcare area to discover drug reactions for patients.

### (ii) [Eclat algorithm](https://towardsdatascience.com/the-eclat-algorithm-8ae3276d2d17):

The Eclat algorithm represents Equivalence Class Transformation. This algorithm needs a depth-first search method to discover frequent itemsets in a transaction database. It implements quicker execution than Apriori algorithm. It does not give us the *confidence* and *lift* metrics that are essential for interpretation in the Apriori algorithm.

### (iii) [FP Growth](https://towardsdatascience.com/the-fp-growth-algorithm-1ffa20e839b8):

There are two faster alternatives to the Apriori algorithm that are state-of-the-art algorithms for frequent itemset mining and basket analysis: one of them is ECLAT and the other one is FP Growth. The F-P stands for Frequent Pattern. It is the enhanced version of Apriori algorithm. It describes the database in the form of a tree structure that is referred to as a frequent pattern or tree.
