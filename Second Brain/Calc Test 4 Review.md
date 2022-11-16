---
tags: Calculus/Test_Review
---

# Sections
1. *15.1 
	1. [[Line Integral]]s
2. *15.2 Calculating 
	1. [[Work]]
	2. [[Vector Field]]s 
	3. [[Flow]] and [[Flux]] across [[Line Integral]]s.
3. *15.3 
	1. [[Conservative]] fields
	2. [[Potential Function]]s/[[Gradient Field]]s/[[Potential Fields]]
4. *15.4*
	1. [[Green's Theorem]]
2. *15.5*
	1. [[Paramaterized Surface Area]]
2. *15.6*
	1. [[Surface Integrals]]

# Important formulas

*[[Line Integral]]:*
$$\int_{S}f(x,y,z)dS=\int_{a}^{b}f(r(t)|\vec v(t)|$$


*[[Work]] (or [[Flow]]) across a [[Vector Field]]:*
$$\int_{S}\vec F \cdot \vec Tds=\int_{a}^{b}\vec F\cdot d\vec r$$

*[[Flux]] across a circular, counterclockwise, region:*
$$\int_{C}\vec F\cdot\vec n=\oint_{C}Mdy-Ndx$$For $y=g(t)$ and $x=h(t)$ for $a\le t\le b$, where that path traces around a circle counterclockwise once

*Fundamental Theorem of Line Integrals:*

For a field $F$ equal gradient fucntion $\nabla f$, over a smooth region $C$,$$\int_{C}F\cdot dr=f(B)-f(A)$$

*Algebraic Proof of [[Conservative]]ness:*

For $F=M(x,y,z)i+N(x,y,z)j+P(x,y,z)k$, if $\frac{\delta P}{\delta y}=\frac{\delta N}{\delta z}$, $\frac{\delta M}{\delta z}=\frac{\delta P}{\delta x}$, and $\frac{\delta M}{\delta y}=\frac{\delta N}{\delta x}$, then $F$ is conservative 

*Flow and Flux of a Simple, Closed, Curve:*

Flow:$$\oint_{C}F\cdot dr=\int\int_{R}(\frac{\delta N}{\delta x}-\frac{\delta M}{\delta y})dxdy$$
Flux:
$$\oint_{C}F\cdot n=\int\int_{R}(\frac{\delta N}{\delta y}+\frac{\delta M}{\delta x})dxdy$$
