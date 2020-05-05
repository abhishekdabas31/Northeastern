# Probabilistic Programming
Conceptually, probabilistic programming languages(PPLs) are domain-specific languages that describe probabilistic models and the mechanics to perform inference in those models. The magic of PPL relies on combining the inference capabilities of probabilistic methods with the representational power of programming languages.

In a PPL program, assumptions are encoded with prior distributions over the variables of the model. During execution, a PPL program will launch an inference procedure to automatically compute the posterior distributions of the parameters of the model based on observed data. In other words, inference adjusts the prior distribution using the observed data to give a more precise mode. The output of a PPL program is a probability distribution, which allows the programmer to explicitly visualize and manipulate the uncertainty associated with a result.

To illustrate the simplicity of PPLs, let’s use one of the most famous problems of modern statistics: a biased coin toss. The idea of this problem is to calculate the bias of a coin. Let’s assume that xi = 1 if the result of the i-th coin toss is head and xi = 0 if it is tail. Our context assumes that individual coin tosses are independent and identically distributed (IID) and that each toss follows a Bernoulli distribution with parameter θ: p(xi = 1 | θ) = θ and p(xi = 0 | θ) = 1 − θ. The latent (i.e., unobserved) variable θ is the bias of the coin. The task is to infer θ given the results of previously observed coin tosses, that is, p(θ | x1, x2, . . . , xN ).

# Deep Probabilistic Programming Language
For decades, the machine learning space was divided in two irreconcilable camps: statistics and neural networks. One camp gave birth to probabilistic programming while the other was behind transformational movements such as deep learning. Recently, the two schools of thought have come together to combine deep learning and Bayesian modeling into single programs. The ultimate expression of this effort is deep probabilistic programming languages(Deep PPLs).

# What is Bayesian machine learning?
To answer this question, it is helpful to first take a look at what happens in typical machine learning procedures (even non-Bayesian ones). In nearly all cases, we carry out the following three steps:
1. Define a model: This is usually a family of functions or distributions specified by some unknown model parameters.
2. Pick a set of data.
3. Run a learning algorithm: This means using the data to choose a value for the unknown model parameters.

## Take deep neural networks as an example: You start with a family of functions with unknown weight parameters, throw in data — usually a large quantity of (input, output) pairs — and then run some gradient-based optimization algorithm (e.g., backpropagation) to get a final set of weights.

# In Bayesian machine learning, we roughly follow these three steps, but with a few key modifications:
1. To define a model, we provide a “generative process” for the data, i.e., a sequence of steps describing how the data was created.
This generative process includes the unknown model parameters.
We incorporate our prior beliefs about these parameters, which take the form of distributions over values that the parameters might take.
2. Data are viewed as observations from the generative process.
3. After running the learning algorithm, we are left with an updated belief about the parameters — i.e., a new distribution over the parameters.

# Why would you want to do this, and when is it useful?
The Bayesian strategy is particularly useful when:
You have prior beliefs about unknown model parameters or explicit information about data generation — i.e., useful info you want to incorporate.
You have few data or many unknown model parameters and it is hard to get an accurate result with your data alone (without the added structure or information).
You want to capture the uncertainty about your result — how sure or unsure your model is — instead of only a single “best” result.
For example, Bayesian learning is used in a variety of industry settings where there are few data and uncertainty quantification is critical, including marketing, advertising, medical product development, pharmaceutical statistics, drug discovery and development, technical recruiting, and computer system A/B testing and tuning.

# A concrete example: Has my milk gone bad?
We can use Bayesian learning in daily life: Suppose I grab a carton of milk from the fridge, see that it is seven days past the expiration date, and want to know if the milk is still good or if it has gone bad. A quick internet search leads me to believe that there is roughly a 50–50 chance that the milk is still good. This is my prior belief.
From past experience, I have some knowledge about how smelly milk gets when it has gone bad. Specifically, let’s suppose I rate smelliness on a scale of 0–10 (0 being no smell and 10 being completely rancid) and have probability distributions over the smelliness of good milk and of bad milk.
Here’s how Bayesian learning works: When I get some data, i.e., when I smell the milk, I can apply the machinery of Bayesian inference to compute an updated belief about whether the milk is still good or has gone bad.
For example, if I observe that the milk is about a 5 out of 10 on the smelly scale, I can then use Bayesian learning to factor in my prior beliefs and the distributions over smelliness of good vs. bad milk to return an updated belief — that there is now a 33% chance that the milk is still good and a 67% chance that the milk has gone bad.

# There are now ways to use new types of model components when defining a Bayesian model or PPL, including:
Deep neural networks .
Simulators — e.g., of scientific processes or equipment.
Visual graphics engines.
Any arbitrary computer program.

Source:-
1. https://towardsdatascience.com/a-gentle-introduction-to-probabilistic-programming-languages-ba9105d9cbce
2. https://medium.com/@Petuum/intro-to-modern-bayesian-learning-and-probabilistic-programming-c61830df5c50