---
tags: Computer_Science/Machine_Learning
---

# Ghist

The forward forward aglorithm (FFA) is a algorithm for training [[Neural Network]]s, similar to [[Backpropogation]], that does not rely on [[Partial Derivative]]s. It does not require a future state.

# Reasoning

In the human brain, no method for backpropogation is known, meaning that our current explenation for NN training seems to be incorrect. [[Gradient Descent]] doesn't seem to be an accurate desriptor of the human learning process. Additionally, alternate learning methods may increase the effeciency and speed of network training - a hot topic in the constantly advaning world of [[Artificial Intelligence]].

# Algorithm

In essentiality, instead of a forards pass of training data combined with a backwards pass of [[Backpropogation]], the network instead trains on two consecutive passes. Each pass is computationally identical, but instead wishes to maximize or mimimize a "goodness function" $G$. Here we will take the goodness to be the sum of the squared neural activities for that layer.

The first pass occurs on real training data. The network attempts to maximize the $G$ for this layer. The second pass occurs on "negative" data, and the network attempts to minimize $G$ for this layer. 

This approach attempts to classify data as being either "positive" or "negative" by generating probabilities of positive or negative data, as $$p(positive)=\sigma (\sum\limits_{j}y_{j}^{2}-\theta)$$(Here, $\sigma$ is the logistic function, $y_j$ is the activity of the hidden layer $j$ as a vector, and $\theta$ is some threshold)

Note that $y_{j}$ is not normalized, but the network normalizes it before passing it to the next layer.

# Example - MNIST

Most networks that are well constructed converge on a jittered [[MNIST]] dataset at about 1.4% accuracy after 20 [[Epoch]]s. In general, this makes a good benchmark, and thus a good target for training a FFN.