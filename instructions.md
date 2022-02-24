# Data Science Technical Exercise Instructions

The purpose of this exercise is to demonstrate your ability to perform exploratory data analysis and feature engineering.

The goal is to predict the likelihood of a new user clicking a given experiences product (such as a tour or cruise) so that we can recommend relevant products to users with no browsing history. New users are given an optional survey in which they may provide their age and a product category that interests them.

Because time is limited, we will constrain the model choice to logistic regression, tuned using 5-fold cross-validation. Your job is to analyze and clean the data and engineer features for the model.

To generate training data, we show users one product at random and record whether they clicked on it.

You are provided with three datasets:

- `users.csv`: Contains survey data from a sample of new users.
- `products.csv`: Contains data about products in a single city.
- `impressions.csv`: Records which users were shown which products and whether they clicked.

The training data, `X_train` and `y_train`, consists of these three datasets merged together.

You are asked to do the following:

1. Analyze the data. Note any data quality issues and interesting findings.
2. Write a `transform()` function that accepts a DataFrame with all of the columns in `X_train` and returns a DataFrame with the features you want to use as model inputs. (You may want to create new features and/or transform existing ones.)
3. Choose a scoring metric to evaluate model performance.

Time permitting, we will train your model and test it on the holdout set in `X_test.csv` and `y_test.csv`.

The exercise template provides a framework for completing the exercise. You are welcome to use anything from numpy, pandas, scikit-learn, provided helper functions, or the Python standard library, and to look up the syntax of any unfamiliar functions.