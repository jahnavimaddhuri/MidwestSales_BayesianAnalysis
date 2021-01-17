# Midwest Sales Bayesian Analysis

During my coursework at UC Irvine, I had learned about Bayesian Analysis and 
worked on this final project to implement some of the new analysis techniques I
had learned! This project uses the Midwest House Sale dataset available in R to 
conduct meaningful analysis on interesting features.

## Goals of Analysis

#### 1. Hypothesis Testing for the proportion of houses with A/C.
For the hypothesis test, I used a null hypothesis of $pi$ $\leq$ 0.8, with an 
alternative hypothesis of $pi$ $>$ 0.8. To conduct this test, I considered the
prior, posterior and likelihood to determine the Bayes Factor. The conclusion
was based on this Bayes Factor.

#### 2. Credible Intervals for the proportion of houses with A/C.
Although the hypothesis testing gave some insights in the proportion of houses 
with A/C. I was interested in inspecting the credible interval for this 
proportion for more precision. For this analysis technique, I used the posterior
to find the credible interval and create an appropriate plot.

#### 3. Predictive Modeling on price based on size.
Next, I used the price and size features in the dataset to predict the price 
of a house based on it's size alone. To conduct predictive modeling, I started
by sampling the data and splitting it into test and train data. I then created 
a normal model using R's stan_glm() function and used this model to predict on 
test data. To compary my predictions with the existing data, I created a 
regression distribution plot where my predictions for y were distributions.