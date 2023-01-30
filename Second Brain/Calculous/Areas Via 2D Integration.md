# Ghist
Part of a series on #Mathematics/Calculus 

Using double [[Integration]], we can find the area of a region through doubling integrals over an area instead of a single integration. This application requires less reasoning about the functions physical properties and is easier to impliment.

# Mathmatics
In general $A=\int\int_RdA$, where the area ($A$) of an integral is an infinite sum of the area of a base shape, summed over two regions of the integral, determined by the boundary of the region given in points, and two functions of $y$ and $x$.

## Examples
### Example 1: Area of region R bounded by $y=x$ and $y=x^2$
```desmos-graph
top = 1;
bottom = 0;
left = 0;
right = 1;
---
y=x
y=x^2
```
$$A=\int_0^1\int_{x^2}^{x}{f(x,y)}dydx$$Here, 0 and 1 are the points where our boundary equations meet. The equivilant with a single interval would have been $$A=\int_0^1(x-x^2)dx$$
### Example 2: Area of R enclosed by $y=x^2$ and $y=x+2$
```desmos-graph
left = -1;
right = 2;
---
y=x+2
y=x^2
```
$$\int_{-1}^{2}\int_{x^2}^{x+2}{f(x)dx}$$Remember that the outer boundaries are found via solving the equation set to find the intersection point, and the inner boundaries are found via the upper and lower function that boundary the region.

### Example 3: Example 2 but horizontal strips
For this solution, you would split the function into two integrals to deal with the regions of the graphs across serperate quadrants

### Example 4: Identifying Regions
Reversing the encoding is trivial, as the inner bounds give you boundary functions, and the outer bounds boudning inputs across those functions.
