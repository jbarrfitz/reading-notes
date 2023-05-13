# Class 13

**Date Due:** April 29, 9am PDT

## Reading

- [_How to Run Linear Regression in Python_](https://www.activestate.com/resources/quick-reads/how-to-run-linear-regressions-in-python-scikit-learn/)
- [_Linear Regression in Python_](https://realpython.com/linear-regression-in-python/)

## Video

- [_Introduction to Simple Linear Regressions_](https://www.youtube.com/watch?v=KsVBBJRb9TE)

## Reading Questions

### Can you explain the basic concept of linear regression and its purpose in the context of machine learning and data analysis?

Linear regression is essentially a model for determining the relationship between
a dependent variable and one or more independent variables. It attempts to establish
a linear pattern that acts as a "best fit" to predict as accurately as possible the
value of a dependent variable based on the the value of the independent ones. In
machine learning and data analysis, this model aids with prediction, the analysis of
trends, and the detection of outlier data points.

### Describe the process of implementing a linear regression model using Python’s Scikit Learn library, including the necessary steps and functions.

1. Import the LinearRegression class
2. Create (or import) the data (such as a NumPy array)
3. Create an instance of a linear regression model. Use the fit() function to fit it to your data.
4. The score() function will produce much meaningful information about the model, including slope and intercept, and it can be used to predict a value

### What is the purpose of splitting the dataset into train and test sets, and how does this contribute to the evaluation of a machine learning model’s performance?

Using one portion of the data to "train" the dataset allows you to still use the other "test" data, to see
how your proposed model deals with data it hasn't yet seen. This can detect whether the proposed model is a good
fit for the data in general. Good performance on the train set accompanied by poor results on the test set may
indicate a problem known as "overfitting," whereby the model is capturing some noise or anomalies that are specific
to the training test set, but not necessarily indicative of all the data as a whole.
