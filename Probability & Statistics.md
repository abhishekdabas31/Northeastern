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
6. Frequency: a number describing how often an outcome occurs. Can be a count like 121801, or a ratio like 0.515.
7. Distribution: A mapping from outcome to frequency for each possible outcome in a sample space.
8. Probability Distribution: The distribution above, which has been normalized so that the sum of the frequencies is 1.

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


## Types of Probabilities
1. Joint Probabilities
The first type of probability we will discuss is the joint probability which is the probability of two different events occurring at the same time. Let’s use the diamonds dataset, from ggplot2, as our example dataset. The two different variables we are interested in are diamond colors and cuts. First we will measure the frequency of each type of diamond color-cut combination. We can represent these data using a “two-way table”:

2. Marginal Probabilities
The second type of probability is the marginal probability. The interesting thing about a marginal probability is that the term sounds complicated, but it’s actually the probability that we are most familiar with. Basically anytime you are in interested in a single event irrespective of any other event (i.e. “marginalizing the other event”), then it is a marginal probability. For instance, the probability of a coin flip giving a head is considered a marginal probability because we aren’t considering any other events. Typically, we just say probability and not the marginal part of it because this part only comes into play when we have to factor in a second event.

3. Conditional Probability
The final type of probability is the conditional probability. A conditional probability is the probability of an event X occurring when a secondary event Y is true. Mathematically, it is represented as P(X | Y). This is read as “probability of X given/conditioned on Y”.

For example, if someone asked you the probability of getting a diamond with the G color, P(X=G), we can use Table 3 to find the marginal probability of this event. But what if you had an additional layer of information where you knew that the diamond was also of ideal cut? This becomes a conditional probability since we have an event that is already true. A conditional probability can be calculated as follows:

P(X | Y)=P(X,Y)/ P(Y)

## Bernoulli theorum 
The Bernoulli distribution is the discrete probability distribution of a random variable which takes a binary, boolean output: 1 with probability p, and 0 with probability (1-p). The idea is that, whenever you are running an experiment which might lead either to a success or to a failure, you can associate with your success (labeled with 1) a probability p, while your insuccess (labeled with 0) will have probability (1-p).
Now, the idea behind the Bernoulli distribution is that the experiment is repeated only once. But what happens if we run more than one trial, under the assumption that trials are independent among each other?
## Binomial theorum
The answer to that question is the Binomial Distribution. This distribution describes the behavior the outputs of n random experiments, each having a Bernoulli distribution with probability p.

Source:-https://towardsdatascience.com/understanding-bernoulli-and-binomial-distributions-a1eef4e0da8f






## Bayes’ Theorem - is perhaps the most important theorem in the field of mathematical statistics and probability theory.
In finance, for example, Bayes’ theorem can be used to rate the risk of lending money to potential borrowers. In medicine, the theorem can be used to determine the accuracy of medical test results by taking into consideration how likely any given person is to have a disease and the general accuracy of the test.





## Hypothesis testing
Hypothesis Tests, or Statistical Hypothesis Testing, 
link:- https://towardsdatascience.com/hypothesis-testing-in-real-life-47f42420b1f7









Sources:-
https://medium.com/ai-techsystems/gaussian-distribution-why-is-it-important-in-data-science-and-machine-learning-9adbe0e5f8ac
https://towardsdatascience.com/why-data-scientists-love-gaussian-6e7a7b726859
https://medium.com/@hemanthsai/gaussian-distribution-for-machine-learning-and-data-science-normal-distribution-bc90139e226d
https://towardsdatascience.com/bayes-theorem-the-holy-grail-of-data-science-55d93315defb