# Ghist
A Kalman filter is an algorithm that can be used to convert several *known states* with weighted probablities into an estimation of an *unkown state*. Its primary use in our context is for finding a [[Cansat Positional Solution]]

# Implimentation
## Mathmatics
One large assumption of the filter is that it is possible to take a variance of the data. We usually do this using the standard deviation $$\sigma=\sqrt{\dfrac{1}{n}\sum{(x_n-\mu)^2}}$$Where $x_n$ is a given value and $\mu$ is the mean of all the values in $x$. In actuatlity we usually measure only a subset of a set, noted as $$\sigma=\sqrt{\dfrac{1}{N-1}\sum{(x_N-\mu)^2}}$$Where $N$ is the number of samples present in the subset. 

Most of the time its very useful to graph out our information in what is known as a [[Normal Distrobution]], into which many natural phenomina fall:$$\dfrac{1}{\sqrt{2\pi\sigma^2}}e^{\dfrac{-(x-\micro)^2}{2\sigma^2}}$$