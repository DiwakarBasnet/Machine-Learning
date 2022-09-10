# Machine-Learning
Machine learning roadmap

## General:-

### Concepts, Inputs & Attributes:
Goal of machine learning is to produce an algorithm that can learn patterns inherent in a dataset to perform specified task.
Put differently, the model learns how to take X(i.e. features or independent variables) in order to predict y(the target or dependent variable).
#### Numeric variables ->
They have values that describe a measurable quantity as a number. It is of 2 types;<br/>
**1. Continuous variable-** Observations can take any value between a set of real numbers. Eg: height, time, age.<br/>
**2. Discrete variable-** Observations cannot take the value of a fraction between one value and the next closest value. Eg; number of members in a family, number of cars, etc.
#### Categorical variables ->
They have values that describe a quality or characteristic of a data unit. It is of 2 types;<br/>
**1. Nominal variable -** It has 2 or more categories, but there is no intrinsic ordering to the categories.<br/>
**2. Ordinal variable -** It is a categorical variable that has clear ordering of the categories.

### Cost functions and gradient descent:
#### Cost function ->
It helps the learner to change behaviour to minimize mistakes. 
A cost function is a measure of how wrong the model is in terms of its ability to estimate the relationship between X and y.
This is typically expressed as a difference or distance between predicted value and actual value.
The cost function can be estimated by iteratively running the model to compare estimated predictions against ground truth (known values of y).
The objective of ML model therefore, is to find parameters, weights or a structure that minimises the cost function.
#### Gradient descent ->
It is an efficient optimization algorithm that attempts to find local or global minima of a function.
![alt text](https://dmol.pub/_images/loss-lr.gif)

### Overfitting and underfitting:
**Overfitting -** too much reliance on training data<br/>
**Underfitting -** a failure to learn relationship in the training data<br/>
**High Variance -** model changes significantly based on training data<br/>
**High Bias -** assumptions about model lead to ignoring training data<br/>
Over and underfitting cause poor generalization on the test set. A validation set for model tuninig can improve under and overfitting.

### Training, validation and test data:
**Training data set -** sample of data used to fit model<br/>
**Validation data set -** sample of data used to fine tune model hyperparameters<br/>
**Test data set -** sample of data used to provide unbiased evaluation of final model fit

### Type I and Type II error:
![alt text](https://www.abtasty.com/wp-content/uploads/type-1-2-errors.png)

### Precision and recall:
Precision and recall are two extremely important model evaluation metrics. While precision refers to the percentage of our results which are relevant, recall refers to the percentage of total relevant results correctly classified by our algorithm. If we have to recall everything, we will have to keep generating results which are not accurate, hence lowering the precision. Unfortunately, it is not possible to maximize both these metrics at the same time, as one comes at the cost of another. For simplicity, there is another metric available called F-1 score. For problems where both precision and recall are important, one can select a model which maximizes this F-1 score. For other problems, a trade-off is needed, and a decision has to be made whether to maximize precision, or recall.

F-1 score = 2 * [(Precision * Recall) / (Precision + Recall)]

### Bias and Variance:
#### Bias- It is a phenomenon that occurs when an algorithm produces results that are prejudice in structural way due to erroneous assumptions in the machine learning process. High bias can cause an algorithm to miss relevant relation between features and target outputs (underfitting). 
If we have high bias problem;
1. Try getting additional features, we are generalizing the datasets.
2. Try adding polynomial features, make the model more complicated.
#### Variance- It is the algorirthm's tendency to learn random things irrespective of the error/noise in the data too closely (overfitting).
If we have high variance problem;
1. We can get more training examples because a larger the dataset is more probable to get a higher predictions.
2. Try smaller sets of features (because we are overfitting).
