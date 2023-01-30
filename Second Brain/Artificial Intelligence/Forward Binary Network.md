---
tags: Computer_Science/Machine_Learning, batshit_insane_idea
---

# Ghist

A potential new [[Machine Learning]] algorithm, based off of a [[Neural Network]] that does not generally utilize [[Backpropogation]] or continous [[Activation]]. It's inspired by the [[Forward Forward Algorithm]], in that it does not utilize a backwards pass, but instead uses several forward passes with differering purposes.

# Structure

As with the [[Feed Forward Network]], the Binary Network (BN) is made up of layers of neurons stacked. However, the binary network differs, in that these layers form planes that are folded back on one another, into a true 3-D form. Layers are packed into different "plate" sizes, and each layer has connections to both the previous layer in the stack, and its accompying layer in the stack below it. This allows for the easier reference of information earlier in the network, without dedicating lanes of neurons across layers soley for passing unobstructed information through, while still allowing for a single, sequential pass to determine the state of the network.

# Activation

Another change meant to resemble the brain's activities is the nature of the neuron. In the [[Feed Forward Network]], the internal value of a layer is calculated with the equation:
$$Z=a^{L-1}w^{L}+b^L$$
Utilizing the previous activations, the neurons weights, and a bias. This is then fed through an activation function that clamps the value of $Z$ between 0 and 1, in order to prevent runaway exponentiation within the network. 

By contract the FBN uses a threshold instead of a bias, and the activation function is:
$$floor[(a^{L-1}+a^{L}_{P-1})\times w^{L}-T^L]$$
This theshold $T$ determines the neuron's "resistance" to firing. Here the $+$ operator denotes the "stacking" of the current previous layer, to the layer one plate below. This, alonsid ethe floor function, creates a binary representation of the neuron, closer anolouging the human brain.

# Input/Output

For the first and last layer, the neurons can be overriden, removing the floor function, in order to extract continuous values from the network.

# Training

To train the BN, backpropogation is not required. Instead two forward passes occur. First, a pass of training data is sent through the network. Second, a pass of feedback data. 

The training data is normal, and the network is evaluated based on a normal [[Cost Function]]. 

The second pass is based on the result of the first pass. If the pass was considered "good" by the trainer, the weights of the neurons that fired are strenghthened by the learning rate, and their thresholds lowered, essentially strengthening those connections. In the opposite case, neurons connections are weakened, and their thresholds raised.