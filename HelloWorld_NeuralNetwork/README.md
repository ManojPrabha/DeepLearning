# DeepLearning
Space to Learn DeepLearning Basics and Try Different stuffs on DeepLearning!!!

Basic structure of Deep Learning model with a single neuron, this can find the relation between two values (y=mx+c)


# Neural Network TensorFlow
## Import Libraries 
import tensorflow as tf
import numpy as np
from tensorflow import keras

## Create a single neuron Network
 model = tf.keras.Sequential([keras.layers.Dense(units=1, input_shape=[1])])
 
## Assign Optimizer and Loss functions to assess the Guess and improve the assumption
model.compile(optimizer='sgd', loss='mean_squared_error')

## Fit the model with number epochs, the number of times it executes, it gets better eventually
model.fit(x, y, epoch=500)

## Finally check prediction
model.predict([10])
