# Supervised Learning:

Supervised learning uses a training set to teach models to yield the desired output. This training dataset includes inputs and correct outputs, which allow the model to learn over time. 
The algorithm measures its accuracy through the loss function, adjusting until the error has been sufficiently minimized.
It can be separated into two types of problems;<br>

## 1. Regression:

It is used to understand the relationship between dependent and independent variables. It is used as an approach to predict continuous outcomes in predictive modelling. Machine learninig regression generally involves plotting a line of best fit through the data points. Regression models could be model that forecasts salary changes, house prices or retail sales. There are a range of different approaches used in machine learning to perform regression. 
Some of the most common regresssion techniques in machine learning can be grouped into following types of regression analysis;

* ### Simple linear regression
It is useful for finding relationship between two continuous variables; one is independent variable and other is dependent variable. It is a technique which plots a straight line within data points to minimise error between the line and data points.

* ### Multiple linear regression
It is a technique that uses more than one independent variables to predict the outcome of a dependent variable.

* ### Polynomial regression
In the previous examples of Linear Regression, when the data is plotted, there was a linear relationship between dependent and independent variables. Thus is was more suitable to build a linear model to get accurate predictions. What if the data points had non-linearity making the linear model give an error in predictions due to non-linearity? 
In this case, we have to build a polynomial relationship which will accurately fit the data points in the given plot.

## 2. Classification: 

It recognizes specific entities within the dataset and attempts to draw some conclusion on how those entities should be labeled. In classification, a program learns from given dataset or observations and then classifies new observation into a number of classes or groups. The best example of ML classification algorithm is Email Spam Detector. The algorithm which implements the classification on the dataset is known as a classifier. There are 2 types of classifer;
- **Binary Classifier:** Classification problem has only 2 possible outcomes
- **Multi-class Classifier:** Classification problem has more than 2 outcomes

There are 2 types of learners in classification;
- **Lazy learners:** Lazy learner stores the training dataset and waits until it receives the test dataset. It takes less time in training but more time for prediction. Example: K-NN algorithm, Case-based reasoning.
- **Eager learners:** Eager learner develop a classification model based on a training dataset before receiving test dataset. It takes more time in learning and less time in prediction. Example: Decision Tree, Naive Bayes, ANN.

* ### Decision Tree
A decision tree is a flowchart-like tree structure where internal node represents features(attributes), the branch represents a decision rule and each leaf node represents the outcome.

* ### Logistic Regression
It is a process of modeling the probability of a discrete outcome given an input variable. Despite its name, it is a classification model rather than regression model. The best way to think about logistic regression is that it is a linear regression but for classification problems. 
