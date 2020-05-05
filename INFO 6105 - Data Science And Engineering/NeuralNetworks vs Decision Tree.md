Supervised and Unsupervised Machine Learning
Methods for analyzing and modeling data can be divided into two groups: “supervised learning” and “unsupervised learning.” Supervised learning requires input data that has both predictor (independent) variables and a target (dependent) variable whose value is to be estimated. By various means, the process “learns” how to model (predict) the value of the target variable based on the predictor variables. Decision trees, regression analysis and neural networks are examples of supervised learning. If the goal of an analysis is to predict the value of some variable, then supervised learning is recommended approach.

Unsupervised learning does not identify a target (dependent) variable, but rather treats all of the variables equally. In this case, the goal is not to predict the value of a variable but rather to look for patterns, groupings or other ways to characterize the data that may lead to understanding of the way the data interrelates. Cluster analysis, correlation, factor analysis (principle components analysis) and statistical measures are examples of unsupervised learning.

Linear Regression

One of the simplest and most popular modeling methods is linear regression. Linear regression fits a straight line (known linear function) to a set of data values. The form of the function fitted by linear regression is:

y = a0 + a1*x1 + a2*x2 + …

Where a0, a1, etc. are parameters whose values are determined so the function best fits the data. Linear regression is a popular modeling technique, and there are many programs available to perform linear regression. However, linear regression is appropriate only if the data can be modeled by a straight line function, which is often not the case. Also, linear regression cannot easily handle categorical variables nor is it easy to look for interactions between variables.

Nonlinear Regression

Nonlinear regression extends linear regression to fit general (nonlinear) functions of the form:

y = f(x1,x2,…,a1,a2,…)

Here are few examples of functions that can be modeled using nonlinear regression:

y = a0 + a1*exp(x1)
y = a0 + a1*sin(x1)

As with linear regression, nonlinear regression is not well suited for categorical variables or variables with interactions. The other challenge involved in using nonlinear regression analysis is that the form (model) of the function must be specified. For engineering and scientific problems, the function model may be dictated by theory, but for marketing, behavioral and medical problems, it can be very difficult to develop an appropriate nonlinear model. The program recommended for linear or nonlinear regression analysis is NLREG

## Logistic Regression

Logistic regression is a variant of nonlinear regression that is appropriate when the target (dependent) variable has only two possible values (e.g., live/die, buy/don’t-buy, infected/not-infected). Logistic regression fits an S-shaped logistic function to the data. As with general nonlinear regression, logistic regression cannot easily handle categorical variables nor is it good for detecting interactions between variables. Classification trees are well suited to modeling target variables with binary values, but – unlike logistic regression – they also can model variables with more than two discrete values, and they handle variable interactions.

## Neural Networks

Neural networks (also called “multilayered perceptron”) provide models of data relationships through highly interconnected, simulated “neurons” that accept inputs, apply weighting coefficients and feed their output to other “neurons” which continue the process through the network to the eventual output. Some neurons may send feedback to earlier neurons in the network. Neural networks are “trained” to deliver the desired result by an iterative (and often lengthy) process where the weights applied to each input at each neuron are adjusted to optimize the desired output.

Neural networks are often compared to decision trees because both methods can model data that has nonlinear relationships between variables, and both can handle interactions between variables. However, neural networks have a number of drawbacks compared to decision trees.

Binary categorical input data for neural networks can be handled by using 0/1 (off/on) inputs, but categorical variables with multiple classes (for example, marital status or the state in which a person resides) are awkward to handle. Classifying a result into multiple categories usually is done by setting arbitrary value thresholds for discriminating one category from another. It would be difficult to devise a neural network to classify the location of residence into the 50 U.S. states. Classification trees, on the other hand, handle this type of problem naturally.

Neural networks do not present an easily-understandable model. When looking at a decision tree, it is easy to see that some initial variable divides the data into two categories and then other variables split the resulting child groups. This information is very useful to the researcher who is trying to understand the underlying nature of the data being analyzed.

A neural network is more of a “black box” that delivers results without an explanation of how the results were derived. Thus, it is difficult or impossible to explain how decisions were made based on the output of the network.

If a challenge is made to a decision based on a neural network, it is very difficult to explain and justify to non-technical people how decisions were made. In contrast, a decision tree is easily explained, and the process by which a particular decision “flows” through the decision tree can be readily shown.

It is difficult to incorporate a neural network model into a computer system without using a dedicated “interpreter” for the model. So if the goal is to produce a program that can be distributed with a built-in predictive model, it is usually necessary to send along some additional module or library just for the neural network interpretation. In contrast, once a decision tree model has been built, it can be converted to if…then…else statements that can be implemented easily in most computer languages without requiring a separate interpreter.



Source:- 
1. https://www.dtreg.com/methodology/view/decision-trees-compared-to-regression-and-neural-networks
2. http://neuralnetworksanddeeplearning.com/chap1.html