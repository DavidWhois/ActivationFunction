# Desirable properties of activation functions
## 1 Non Linearity
The purpose of the activation function is to introduce non-linearity into the network in turn allows you to model a response variable (aka target variable, class label, or score) that varies non-linearly with its explanatory variables
Non-linear means that the output cannot be reproduced from a linear combination of the inputs
Another way to think of it: without a non-linear activation function in the network, a NN, no matter how many layers it had, would behave just like a single-layer perceptron, because summing these layers would give you just another linear function (see definition just above).
## 2Continuously differentiable
This property is necessary for enabling gradient-based optimization methods.
The binary step activation function is not differentiable at 0, and it differentiates to 0 for all other values, so gradient-based methods can make no progress with it
## 3 Range
When the range of the activation function is finite, gradient-based training methods tend to be more stable, because pattern presentations significantly affect only limited weights.
When the range is infinite, training is generally more efficient because pattern presentations significantly affect most of the weights. In the latter case, smaller learning rates are typically necessary.
## 4 Monotonic
When the activation function is monotonic, the error surface associated with a single-layer model is guaranteed to be convex.
## 5 Approximates identity near the origin
When activation functions have this property, the neural network will learn efficiently when its weights are initialized with small random values.
When the activation function does not approximate identity near the origin, special care must be used when initializing the weights.
