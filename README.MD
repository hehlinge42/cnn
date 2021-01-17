# Training CNNs on CIFAR-10

This project was completed by Hugo Hellainger, Louis Bertolotti and Nicolas Maisonneuve-Bonteil during the "Deep Learning" course of the X-HEC Joint Degree "Data Science for Business". 

## Goal

The goal of this project was to find the CNN trained on the [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html) with the best balance of accuracy and computation time. Starting with a naïve model, we enhanced it and then compared it to a pre-trained model (InceptionResNetV2) which we adapted to our image input size.

We reached a final accuracy of 0.74 with a reasonable computation time.

## Technologies

The Keras and Tensorflow libraries were used to create the models. We also decided to make full use of the Tensorboard API, which collects logs on the model and helps to analyse parameters such as the number of epochs or the model accuracy.

## Detailled informations

The notebook contains a custom class called "UniversalHPOptimizer", which runs a GridSearch with given parameters and automatically returns the best model. It leverages the Tensorboard-compatible HParams data format, allowings callbacks to return information to Tensorboard.