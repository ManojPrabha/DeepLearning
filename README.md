# DeepLearning
Space to Learn DeepLearning Basics and Try Different stuffs on DeepLearning!!!


# Basics of Neural Network

## Neuron:
 A neuron forms the basic structure of a neural network. A neuron receives an input, processes it and generates an output which is either sent to other neurons for further processing or it is the final output.

## Neural Network:
 Neural Networks form the backbone of deep learning.The goal of a neural network is to find an approximation of an unknown function. It is formed by interconnected neurons. These neurons have weights, and bias which is updated during the network training depending upon the error. The activation function puts a nonlinear transformation to the linear combination which then generates the output. The combinations of the activated neurons give the output.
 
## Weights:
 When input enters the neuron, it is multiplied by a weight. We initialize the weights randomly and these weights are updated during the model training process. The neural network after training assigns a higher weight to the input it considers more important as compared to the ones which are considered less important. A weight of zero denotes that the particular feature is insignificant.
 
## Bias:
 In addition to the weights, another linear component is applied to the input, called as the bias. It is added to the result of weight multiplication to the input. The bias is basically added to change the range of the weight multiplied input. After adding the bias, the result would look like a*W1+bias. This is the final linear component of the input transformation.
 
## Activation:
 The role of the Activation Function is to derive output from a set of input values fed to a node (or a layer). The primary role of the Activation Function is to transform the summed weighted input from the node into an output value to be fed to the next hidden layer or as output.
 
 
a) Sigmoid  -  One of the most common activation functions used is Sigmoid. The sigmoid transformation generates a more smooth range of values between 0 and 1. We might need to observe the changes in the output with slight changes in the input values. Smooth curves allow us to do that and are hence preferred over step functions.

sigmoid(x) = 1/(1+e^-x)
 
b) ReLU(Rectified Linear Units) – Instead of sigmoids, the recent networks prefer using ReLu activation functions for the hidden layers. The major benefit of using ReLU is that it has a constant derivative value for all inputs greater than 0. The constant derivative value helps the network to train faster.

f(x) = max(x,0)
 
c) Softmax - Softmax activation functions are normally used in the output layer for classification problems. It is similar to the sigmoid function, with the only difference being that the outputs are normalized to sum up to 1. The sigmoid function would work in case we have a binary output, however in case we have a multiclass classification problem, softmax makes it really easy to assign values to each class which can be easily interpreted as probabilities.

## Forward Propagation:
 Forward Propagation refers to the movement of the input through the hidden layers to the output layers. In forward propagation, the information travels in a single direction FORWARD. The input layer supplies the input to the hidden layers and then the output is generated. There is no backward movement.
 
## Backpropagation:
 When we define a neural network, we assign random weights and bias values to our nodes. Once we have received the output for a single iteration, we can calculate the error of the network. This error is then fed back to the network along with the gradient of the cost function to update the weights of the network.
 
 ## Epochs:
  An epoch is defined as a single training iteration of all batches in both forward and back propagation. This means 1 epoch is a single forward and backward pass of the entire input data.
  
## Batch Normalization:
 As a concept, batch normalization can be considered as a dam we have set as specific checkpoints in a river. This is done to ensure that distribution of data is the same as the next layer hoped to get. When we are training the neural network, the weights are changed after each step of gradient descent.
