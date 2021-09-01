# Starbucks-capstone-project
This project is the final project in the Udacity Machine Learning Engineering nanodegree.
Here we are working on Starbucks data, offers and discounts have always been known as effective tools at increasing sales and attracting customers.
But not all offers are created equal and different customers have different tastes. In this project we will be using machine learning to make better choices about
which offers to send.
Given a dataset of customer info, offers info and a log of transactions and interactions with offers of the past month, we will train a model that – given a customer and an offer- tries to
predict whether that customer will respond to that offer.
Responding to an offer means viewing the offer and then making the required transactions to complete it while it is active.
We will first preprocess, clean and encode the data to the required form for the model.
We will then train the model with said data and evaluate our predictions on test data.


A logistic regression algorithm will be used in this project as a benchmark model, because it is a simple model and I expect CatBoost to be able to beat it.
After applying preprocessing (discussed below) and training the model I achieved an accuracy score of about 0.825, which will be our target to beat.

The CatBoostClassifier class model is pretty straightforward and has a default values for all parameters and the project is simple and standard enough that the default values take care of
the problem. That being said there is an important parameter, which is iterations.
The default value of it is 1000, but I decided to change it and see how the accuracy would react. In the end I decided on values below (explanation in the next section, refinement): Iteration = 350
Learning rate = 0.126 (decided by the model based on iteration value)
P.S. You will need to install catboost usnig (!pip3 install catboost) on your notebook, you will find this in the first cell in the notebook.
