# Data Science Technical Exercise Instructions

The purpose of this exercise is to demonstrate your ability to perform exploratory data analysis and feature engineering.

The goal is to predict the likelihood of a new user clicking a given experiences product (such as a tour or cruise) so that we can recommend relevant products to users with no browsing history. New users are given an optional survey in which they may provide their age and a product category that interests them.

To generate training data, we showed users one product at random and recorded whether they clicked on it.

Because time is limited, we will constrain the model choice to logistic regression. Your job is to analyze the data and engineer features for the model.

You are provided with three datasets:

- `users.csv`: Contains survey data from a sample of new users.
- `products.csv`: Contains data about products in a single city.
- `impressions.csv`: Records which users were shown which products and whether they clicked.

You are asked to do the following:

1. Analyze the data. Note any data quality issues and interesting findings. (~20 min)
2. Describe the features you want to use in your model. You can use pseudocode or English rather than writing code. (~10 min)
3. Explain what the code in the "Model training" section does. We may ask a few follow-up questions. (~10 min)

The notebook provides a framework for completing the exercise. You are welcome to look up unfamiliar syntax or ask your interviewer for help.