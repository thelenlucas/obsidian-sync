---
tags: Calculus
---
# Ghist
Sometimes, we may wish to determine the value of a function over a set of parameters in [[3-D Space]], in order to tdo this, we may performe [[Integration]] over a [[Parametric Equation]] set for a given function. For a paramaterization $r(t)$, we evaluate this as $$\int_{a}^{b}f(r_{x}(t), r_{y}(t),r_{z}(t))\cdot|\vec v(t)|dt$$
# Properties
Line integrals may be added from each other on continuous flows. $$\int_{C}=\int_{C_{0}}+\int_{C_{1}}$$

# Example
Say we have a function $f(x,y)$ that we wish to integrate over a parabola in the 2-D plane $xy$, in the [[Cartesian Coordinate System]], over the curve $y=x^2$, with a function of $f=2x+y$. We may easily paramatarize the curve to $$r(t)=(t)i+(t^{2})j\space\space0\leq t\leq1$$We then substitute in for the function to get $$f(r(t))=2t+t^{2}$$And then take the first order to get $$|\vec v(t)|=\sqrt{1^2+(2t)^2}$$
Integrate as normal for $$\int_{0}^{1}(2t+t^2)\sqrt{4t^{4}+1}$$