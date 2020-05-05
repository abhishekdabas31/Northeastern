# Machine Learning models have one sole purpose that is to generalize well.

## What is meant by Generalization??
Generalization is the model’s ability to give sensible outputs to sets of input that it has never seen before. If the model generalizes well, it serves its purpose.

Coming to the Topic: Overfitting and Underfitting
## overfitting and underfitting refer to deficiencies that the model’s performance might suffer from.
This simply means to knowing “how off” the model’s predictions are......is a matter of knowing how close it is to overfitting or underfitting.

# Hence a model that generalizes well is a model that is neither underfit nor overfit.

## Overfitting
When we run our training algorithm on the data set, we allow the overall cost (i.e. distance from each point to the line) to become smaller with more iterations. Leaving this training algorithm run for long leads to minimal overall cost. However, this means that the line will be fit into all the points (including noise), catching secondary patterns that may not be needed for the generalizability of the model.
 
The essence of an algorithm like Linear Regression is to capture the dominant trend and fit our line within that trend. In the figure above, the algorithm captured all trends — but not the dominant one. If we want to test the model on inputs that are beyond the line limits we have (i.e. generalize), what would that line look like? There is really no way to tell. Therefore, the outputs aren’t reliable. If the model does not capture the dominant trend that we can all see (positively increasing, in our case), it can’t predict a likely output for an input that it has never seen before — defying the purpose of Machine Learning to begin with!

# Overfitting is the case where the overall cost is really small, but the generalization of the model is unreliable. This is due to the model learning “too much” from the training data set.
The more we leave the model training the higher the chance of overfitting occurring. We always want to find the trend, not fit the line to all the data points. Overfitting (or high variance) leads to more bad than good.

## Underfitting
We want the model to learn from the training data, but we don’t want it to learn too much (i.e. too many patterns). One solution could be to stop the training earlier. However, this could lead the model to not learn enough patterns from the training data, and possibly not even capture the dominant trend. This case is called underfitting.
# Underfitting is the case where the model has “ not learned enough” from the training data, resulting in low generalization and unreliable predictions.

underfitting (i.e. high bias) is just as bad for generalization of the model as overfitting. 

# Bias-variance trade-off
> So what is the right measure? 
Depending on the model at hand, a performance that lies between overfitting and underfitting is more desirable. This trade-off is the most integral aspect of Machine Learning model training. As we discussed, Machine Learning models fulfill their purpose when they generalize well. Generalization is bound by the two undesirable outcomes — high bias and high variance. Detecting whether the model suffers from either one is the sole responsibility of the model developer

## what is a model?
A model is simply a system for mapping inputs to outputs. For example, if we want to predict house prices, we could make a model that takes in the square footage of a house and outputs a price. A model represents a theory about a problem: there is some connection between the square footage and the price and we make a model to learn that relationship. Models are useful because we can use them to predict the values of outputs for new data points given the inputs.
A model learns relationships between the inputs, called features, and outputs, called labels, from a training dataset. During training the model is given both the features and the labels and learns how to map the former to the latter. A trained model is evaluated on a testing set, where we only give it the features and it makes predictions. We compare the predictions with the known labels for the testing set to calculate accuracy. Models can take many shapes, from simple linear regressions to deep neural networks, but all supervised models are based on the fundamental idea of learning relationships between inputs and outputs from training data.

# Training and Testing Data
To make a model, we first need data that has an underlying relationship. For this example, we will create our own simple dataset with x-values (features) and y-values (labels). An important part of our data generation is adding random noise to the labels. In any real-world process, whether natural or man-made, the data does not exactly fit to a trend. There is always noise or other variables in the relationship we cannot measure. In the house price example, the trend between area and price is linear, but the prices do not lie exactly on a line because of other factors influencing house prices.
Our data similarly has a trend (which we call the true function) and random noise to make it more realistic. After creating the data, we split it into random training and testing sets.

# A model that is underfit will have high training and high testing error while an overfit model will have extremely low training error but a high testing error.

Source:
1. https://towardsdatascience.com/what-are-overfitting-and-underfitting-in-machine-learning-a96b30864690
2. https://towardsdatascience.com/overfitting-vs-underfitting-a-conceptual-explanation-d94ee20ca7f9
3. https://towardsdatascience.com/overfitting-vs-underfitting-a-complete-example-d05dd7e19765