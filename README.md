# AI
This is my first application of Neural Network (NN) using the book Neural Networks and Deep Learning by Michael A. Nielsen (http://neuralnetworksanddeeplearning.com). 
In this source, I designed and built a feed-forward neural network to recognize handwritten digits using the MNIST handwritten digits dataset. The MNIST database of handwritten digits, available from this page (http://yann.lecun.com/exdb/mnist/), has a training set of 60,000 examples, and a test set of 10,000 examples. It is a subset of a larger set available from NIST. The digits have been size-normalized and centered in a fixed-size image.

Each data is an array containing the image data (28 x 28 pixels) and the corresponding output digit output[0...9]. I built a 3 layer NN with 784 input neurons, 10 output neurons and a varying number of hidden layer neurons (1 - 100). I also increased the depth of the network by adding more hidden layers, to see if there would be significant improvement in accuracy --but this didn't necessarily translate into more accuracy (obviously).

The weights (w) and biases (b) of the neurons are updated using Stochastic Gradient Descent (SGD) with the data randomly sampled in batches to increase the speed of the algorithm. I used quadratic cost function(C), which is simply the Mean Squared Error (MSE) between the output from the network and the actual(or supposed) output in the dataset. To improve the accuracy of the algorithm, the cost function should be minimized to the barest minimum. This is where SGD comes in; Gradient Descent (GD) minimizes a function by computing the gradients of all the dimesions of the function and moving in the opposite direction in each dimension. SGD is an optimized variant of GD whereby random samples of the input data are batched and each batch is minimized by the algorithm --the overall minimization of the function is the average of all the batch minimizations. This greatly improves the speed of the algorithm.

Gradient Descent uses an algorithm called Back Propagation to compute the partial derivates of the cost function. 




