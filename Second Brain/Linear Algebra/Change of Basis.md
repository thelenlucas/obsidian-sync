---
tags: Mathematics/Linear_Algebra
---

In $R^n$, we represent our coordinates using the [[Standard Basis]], or some other [[Vector Span]] that covers a  [[Vector Space]].

Let $B=\{v_{1},v_{2},\cdot\cdot\cdot,v_{n}\}$ be the ordered basis for a space $V$. Lets say we have a vector $x$ so that $$x=c_{1}v_{1}+c_{2}v_{2}+ \cdot\cdot\cdot+c_{n}v_{n}$$The scalars $c_n$ are the **coordinates of $x$ relative to the basis $B$.** The **Coordinate Matrix** of $x$ relative to $B$ is a column matrix in $R^n$ that is $$[x]_{B}=\begin{bmatrix}c_{1}\\c_{2}\\\cdot\cdot\cdot\\c_{n}\end{bmatrix}$$Column notation is used because it makes [[Matrix]] multiplication easy.

To transition between the standard basis $B$ and a non-standard basis $B'$, we use a [[Transition Matrix]] $P$. We write this as $$P[x]_{B'}=[x]_{B}$$To create the [[Transition Matrix]] we use the formula$$\begin{bmatrix}B&B'\end{bmatrix}=\begin{bmatrix}I&P^{-1}\end{bmatrix}$$