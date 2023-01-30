# Gradient Descent

A calculus technique that utilizes vectors to minimize a function given a set of inputs. Calculated by taking the partial of a function with respect to one of its inputs, then tweaking the parameters of that value in respect to that vector value. Usually implimented via iterating over all parameters, tweaking, and then repeating.

### Practical

Used extensively in [[Machine Learning]] to minimize a given [[Cost Function]]'s value for an input. Usually the tweaking vector $v$ is calculated as $$v=\dfrac{1}{n}\sum{C_0(P_0)}$$This allows us to ignore the summation function in our parametric solutions, for those algorithms with no trivial partial solution.