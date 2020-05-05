# Probability Distribution in Data Science
Having a sound statistical background can be greatly beneficial in the daily life of a Data Scientist. Every time we start exploring a new dataset, we need to first do an Exploratory Data Analysis (EDA) in order to get a feeling of what are the main characteristics of certain features. If we are able to understand if it’s present any pattern in the data distribution, we can then tailor-made our Machine Learning models to best fit our case study. In this way, we will be able to get a better result in less time (reducing the optimisation steps). In fact, some Machine Learning models are designed to work best under some distribution assumptions. Therefore, knowing with which distributions we are working with, can help us to identify which models are best to use.


## Numerical data can additionally be divided into other two categories: Discrete and Continue. Discrete data can take only certain values (eg. number of students in a school) while continuous data can take any real or fractional value (eg. the concepts of height and weights).


## Bernoulli Distribution
The Bernoulli distribution is one of the easiest distributions to understand and can be used as a starting point to derive more complex distributions.
This distribution has only two possible outcomes and a single trial.
A simple example can be a single toss of a biased/unbiased coin. In this example, the probability that the outcome might be heads can be considered equal to p and (1 - p) for tails (the probabilities of mutually exclusive events that encompass all possible outcomes needs to sum up to one).

## Uniform Distribution
The Uniform Distribution can be easily derived from the Bernoulli Distribution. In this case, a possibly unlimited number of outcomes are allowed and all the events hold the same probability to take place.
As an example, imagine the roll of a fair dice. In this case, there are multiple possible events with each of them having the same probability to happen

## Binomial Distribution
The Binomial Distribution can instead be thought as the sum of outcomes of an event following a Bernoulli distribution. The Binomial Distribution is therefore used in binary outcome events and the probability of success and failure is the same in all the successive trials. This distribution takes two parameters as inputs: the number of times an event takes place and the probability assigned to one of the two classes.
A simple example of a Binomial Distribution in action can be the toss of a biased/unbiased coin repeated a certain amount of times.

### The main characteristics of a Binomial Distribution are:
Given multiple trials, each of them is independent of each other (the outcome of one trial doesn’t affect another one).
Each trial can lead to just two possible results (eg. winning or losing), which have probabilities p and (1 - p).

## Normal (Gaussian) Distribution
The Normal Distribution is one of the most used distributions in Data Science. Many common phenomena that take place in our daily life follows Normal Distributions such as: the income distribution in the economy, students average reports, the average height in populations, etc… In addition to this, the sum of small random variables also turns out to usually follow a normal distribution (Central Limit Theorem).

### Some of the characteristics which can help us to recognise a normal distribution are:
The curve is symmetric at the centre. Therefore mean, mode and median are all equal to the same value, making distribute all the values symmetrically around the mean.
The area under the distribution curve is equal to 1 (all the probabilities must sum up to 1).

# Poisson Distribution
Poisson Distributions are commonly used to find the probability that an event might happen or not knowing how often it usually occurs. Additionally, Poisson Distributions can also be used to predict how many times an event might occur in a given time period.
Poisson Distributions are for example frequently used by insurance companies to conduct risk analysis (eg. predict the number of car crash accidents within a predefined time span) to decide car insurance pricing.
When working with Poisson Distributions, we can be confident of the average time between the occurrence of different events, but the precise moment an event might take place is randomly spaced in time.
A Poisson Distribution can be modelled using the following formula (Figure 9), where λ represents the expected number of events which can take place in a period.

# The main characteristics which describe Poisson Processes are:
The events are independent of each other (if an event happens, this does not alter the probability that another event can take place).
An event can take place any number of times (within the defined time period).
Two events can’t take place simultaneously.
The average rate between events occurrence is constant.


# Exponential Distribution
Finally, the Exponential Distribution is used to model the time taken between the occurrence of different events.
As an example, let’s imagine we work at a restaurant and we want to predict what is going to be the time interval between different customers coming to the restaurant. Using an Exponential Distribution for this type of problem, could be the perfect place where to start.
Another common application of Exponential distributions is survival analysis (eg. expected life of a device/machine).
Exponential distributions are regulated by a parameter λ. The greater the value of λ and the faster the exponential curve is going to decade.





Source:- 
1. https://towardsdatascience.com/probability-distributions-in-data-science-cce6e64873a7