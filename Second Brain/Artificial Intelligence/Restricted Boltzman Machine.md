---
tags: Computer_Science/Machine_Learning
---

# Ghist

Boltzman Machines (BMs), are a type of [[Neural Network]] that are trained with [[Stochastic]] methods to learn probability distrobutions over a set of inputs.

# Structure

The network consists of two layers, one made outof inputs, and one [[Hidden Layer]]-esque hidden unit layer. Both the input and hidden units are boolean, they do not carry continuous values. Visible and hidden units are represented as matrices, and individually as $v_{j}$ and $h_j$, respectively.

The connections between the layers are represented by a [[Matrix]] of weights $W$. $W$ is of size $v\times h$. There are additionally two matrices $a$ and $b$ that serve as static biases for the network. 

To find the prediction of a network, first the energy is taken as 
$$E(v,h)=-a^{T}v-b^{T}h-v^{T}Wh$$
Then, the probability of the current state is calculated as
$$P(v,h)=\frac{1}{Z}e^{-E(v,h)}$$
Where $Z$ is the sum of all possible results of $E$. 

### Image
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Restricted_Boltzmann_machine.svg/800px-Restricted_Boltzmann_machine.svg.png">




# Training

 