# K-Nearest Neighbours Algorithm
The k-nearest neighbours (KNN) algorithm is a simple, easy to implement supervised machine learning algorithm 
that can be used to solve both classification and regression problems.
The KNN algorithm assumes that similar things exist in close proximity. In other words, similar things are near to each other.

## The KNN algorithm:
1. Load the data
2. Initialize K to your chosen number of neighbours
3. For each example in data
  3.1 Calculate the distance between the query example and current example from the data
  3.2 Add the distance and the index of the example to an ordered collection
4. Sort the ordered collection of distances and indices from smallest to largest by distances
5. Pick the first K entries from the sorted collection
6. Get the labels of the selected K entries
7. If regression, return mean of the K labels
8. If classification, return mode of the K labels

## Choosing the right value of K:
To select the K that's right for your data, we run the KNN algorithm several times with different values of K and
choose the K that reduces the number of errors we encounter while maintaining the algorithm's ability to accurately
make predictions when it's given data it hasn't seen before.
Some things to keep in mind-
1. As we decrease the value of K to 1, our predictions become less stable.
2. Inversely, as we increase the value of K, our predictions become more stable up to a certain point. Eventually,
   we begin to witness an increasing number of errors.
3. In cases where we are taking a majority vote like in a classification problem, we usually make K an odd number
   to have a tiebreaker.

  In case of large data value of K can be square root of number of data points.
