# Nerual Networks

A tuned function approximater. A very powerful [[Machine Learning]] algorithm that has spawned many powerful applications such as [[GPT-3]].

Part of a series on #machine_learning 

# Explenation
A Neural network is a construct of individual simulated neurons, that fire based of an internal state generated from the previous layer's outputs. It has a single input and output layer, and $n>0$ internal [[Hidden Layer]]s. <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Neural_network_example.svg/800px-Neural_network_example.svg.png">

# Mathematics
Nominally, for each neuron there are two equations that determine the neuron's output:
1. $z^{(L)}=\sum\limits{a^{(L-1)}_{n}w^{(L)}_n}+b$
2. $a^{(L)}=A(z^{(L)})$

Here, $a$ is the activation of the some layer, $z$ is the internal state of the neuron, and $A$ is some [[Activation Function]] such as the [[Sigmoid Function]]. The entire network can be evaluated by calling it's output through a [[Cost Function]], usually denoted as $C_0$ for a single example, and $C$, more generally.

## Matrix Representation
Usually, it's much more expedient to refer to these networks via [[Matrix]]es. To do so, we refer to layers via a superscript $(L-n)$, where $n$ is the distance from the last layer. For example, $a^{(L)}$ is the activations of the outer layer, $z^{(L-1)}$ is the internal state of the neurons in the layer second to last and $w^{(L-2)}$ is the weights of the neurons in the layer third from the last layer. All of these values are matrixes, where we refer expecially to the $z$ and $a$ values of each layer as verticle matrices with the number of rows determined by the neuron count. For example, the layer $L$'s activation values $a$, with two neurons of output, looks like $$
a^{(L)}=\begin{matrix}a^{(L)}_j \\ a_k^{(L)} \end{matrix}$$[^1]

We then define weights for each layer as a matrix with the dimensions (number of neurons in the previous layer) $\times$ (number of neurons in this layer). Say layer $(L-1)$ has three neurons in it, and $(L)$ is the same as before. The weights $w^{(L)}$ would then be arranged$$w^{(L)} = \begin{matrix}w_{jj} & w_{jk} & w_{jl} \\ w_{kj} & w_{kk} & w_{kl}\end{matrix}$$
This representation allows us, via the rules of [[Matrix Multiplication]] and [[Matrix Addition]], to perform the same operations as we did previously, this time defining them as 
1. $z^{(L)}=w^{(L)}a^{(L-1)}+b^{L}$
2. $a^{(L)}=A(z^{(L)})$

[^1]: The biases $b^{(L)}$ are defined the same way