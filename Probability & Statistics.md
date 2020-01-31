# Probability & Statistics


## Basics:
1. Dependent variable :-
A dependent variable is the variable being tested and measured in a scientific experiment.
2. Independent variables :- 
An independent variable is the variable that is changed or controlled in a scientific experiment to test the effects on the dependent variable.
`example:`
The brightness of the light is controlled by the scientist. This would be the independent variable. How the moth reacts to the different light levels (distance to light source) would be the dependent variable.
3. Standard Deviation:-
Standard deviation tells about the concentration of the data around the mean of the data set.Standard deviation is inversely proportional to the concentration of the data around the mean, as the more data is near the mean the less the standard deviation would be.
4. Variance :-
Variance is the measure of dispersion in a data set, or basically how spread out the dataset is.
`Calculated by-` first finding the deviation of each element in the data set from the mean, and then by squaring it.
5. Lambda :-
In python, the lambda keyword to declare an anonymous function, which is why we refer to them as "lambda functions"


## Intermediate
1. Gaussian Distribution :-
`For Deep Learning & Machine Learning engineers out of all the probabilistic models in the world, Gaussian distribution model simply stands out.`
`Gaussian distribution model, often identified with its iconic bell shaped curve, also referred as Normal distribution` 
Incredible number of processes in nature and social sciences naturally follows the Gaussian distribution. Even when they don’t, the Gaussian gives the best model approximation for these processes. Some examples include-
Our height, blood pressure of adult human and intelligence
Position of a particle that experiences diffusion
Measurement errors


2. Normal Distribution :-
'Distribuition' - It is a collection of value and frequency about a given observation like the age in population
The statistical term for Normal Distribution is Gaussian distribution, but many people call it the Bell Curve as it is shaped like a bell
The highest point is located at the mean, because it coincides with the mode. The spread of the graph is determined by the standard deviation
We have two main paramters to explain or inform regarding our Gaussian distribution model they are mean and variance. Mean is usually represented by μ and variance with σ² (σ is the standard deviation). The graph is symmetrix about mean for a gaussian distribution. The mean, median and mode are equal
`While usually modelling a large data it is common that more data is closer to the mean value and the very few or less frequent data is observed towards the extremes, which is nothing but a gaussian distribution that looks like this(μ = 0 and σ = 1):`

The central limit theorem (CLT) establishes that, in some situations, when independent random variables are added, their properly normalized sum tends toward a normal distribution (informally a “bell curve”) even if the original variables themselves are not normally distribute
### So because of these properities and Central Limit Theorem (CLT), Gaussian distribution is often used in Machine Learning Algorithms.
### In summary, it is possible to turn most datasets to Gaussian.

## Why are They Important to Machine Learning?
In machine learning, cost function or a neuron potential values are the quantities that are expected to be the sum of many independent processes (such as input features or activation potential of last layer) often have distributions that are nearly normal. One can continue to use parametric statistics knowing gaussian nature of dataset.





















Sources:-
https://medium.com/ai-techsystems/gaussian-distribution-why-is-it-important-in-data-science-and-machine-learning-9adbe0e5f8ac
https://towardsdatascience.com/why-data-scientists-love-gaussian-6e7a7b726859
https://medium.com/@hemanthsai/gaussian-distribution-for-machine-learning-and-data-science-normal-distribution-bc90139e226d