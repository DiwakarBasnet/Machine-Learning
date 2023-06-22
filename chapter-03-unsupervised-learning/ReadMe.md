# Unsupervised Learning:

Unsupervised learning refers to algorithms that learn patterns from unlabeled data.
In contrast to supervised learning where models learn to map the input to the target output, unsupervised methods learn concise representations of the input data, which can be used for data exploration or to analyze or generate new data.
The algorithms used in unsupervised learning can mainly be categorized into three types, they are;<br>

## 1. Clustering:

Using clustering algorithm means we're going to give the algorithm a lot of input data with no labels and let it find any groupings in the data it can. Those groupings are called clusters. A cluster is a group of data points that are similar to each other based on their relation to surrounding data points.
Clustering is used for things like feature engineering or pattern discovery. When we're starting with data we know nothing about, clustering might be a good place to get some insight.
Types of clustering algorithm;<br>

### (I) Hierarchical clustering:

This clustering technique is further divided into two types:<br>
* Agglomerative Hierarchical clustering - In this technique, initially each data point is considered as an individual cluster. At each iteration, the similar clusters merge with other clusters until one cluster or K clusters are formed.<br>
* Divisive Hierarchical clustering - In simple words, we can say that the Divisive Hierarchical clustering is exactly the opposite of the Agglomerative Hierarchical clustering. In Divisive Hierarchical clustering, we consider all the data points as a single cluster and in each iteration, we separate the data points from the cluster which are not similar. Each data point which is separated is considered as an individual cluster. In the end, we’ll be left with n clusters.<br>

### (II) K-Means clustering:

