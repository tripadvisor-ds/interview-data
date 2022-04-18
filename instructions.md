# Data Science Technical Exercise Instructions

The purpose of this exercise is to demonstrate your ability to perform exploratory data analysis and feature engineering.

The goal is to predict the likelihood of a new user clicking a given experiences product (such as a tour or cruise) so that we can recommend relevant products to users with no browsing history. New users are given an optional survey in which they may provide their age and a product category that interests them.

Because time is limited, we will constrain the model choice to logistic regression. Your job is to analyze the data and engineer features for the model.

To generate training data, we show users one product at random and record whether they clicked on it.

You are provided with three datasets:

- `users.csv`: Contains survey data from a sample of new users.
- `products.csv`: Contains data about products in a single city.
- `impressions.csv`: Records which users were shown which products and whether they clicked.

The training data, `X_train` and `y_train`, consists of these three datasets merged together.

You are asked to do the following:

1. Analyze the data. Note any data quality issues and interesting findings.
2. Edit the `transform()` function to generate the features that you want to use in your model. `transform()` will be applied to the raw data at both train and predict time.
   - To save time, commented-out code has been provided, but you should not use all of it. Uncomment the lines that you do want to use and explain your thinking.
   - Optionally, you may suggest features for which code is not provided.
3. Choose a scoring metric to evaluate model performance.

Time permitting, we will train your model and test it on the holdout set in `X_test.csv` and `y_test.csv`.

The exercise template provides a framework for completing the exercise. You are welcome to look up unfamiliar syntax or ask your interviewer for help.