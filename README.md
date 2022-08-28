# Machine-Learning
Machine learning roadmap

## General:-
### Concepts, Inputs & Attributes:
Goal of machine learning is to produce an algorithm that can learn patterns inherent in a dataset to perform specified task.
Put differently, the model learns how to take X(i.e. features or independent variables) in order to predict y(the target or dependent variable).

#### Numeric variables ->
They have values that describe a measurable quantity as a number. It is of 2 types;<br />
**1. Continuous variable-** Observations can take any value between a set of real numbers. Eg: height, time, age.<br />
**2. Discrete variable-** Observations cannot take the value of a fraction between one value and the next closest value. Eg; number of members in a family, number of cars, etc.

#### Categorical variables ->
They have values that describe a quality or characteristic of a data unit. It is of 2 types;<br />
**1. Nominal variable -** It has 2 or more categories, but there is no intrinsic ordering to the categories.<br />
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
