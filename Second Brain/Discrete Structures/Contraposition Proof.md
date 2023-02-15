---
tags: Mathematics/Discrete_Structures
---

# Ghist

One of the many forms of [[Proof]], the contrapositive strategy attemts to establish a [[Propositional Logic]] via [[De Morgans]] theorem. That is, to prove $P \rightarrow Q$ via $Q' \rightarrow P'$.

# Example

Prove: For all ingagers $n$, if $n^2$ is even, then $n$ is even. 

Our original statement consisted of: If $n^2$ is even $\rightarrow$ $n$ is even. If we take the contropositive of this, we find: If $n$ is odd $\rightarrow$ $n^2$ is odd. If we can prove this, it will prove the original theorem as $$(Q'\rightarrow {P'}) \rightarrow (P\rightarrow Q)$$Now we know that our goal is to prove that if $n$ is not even (odd), then $n^2$ is not even (odd):

1. Suppose $n$ is odd
2. In that case, $n$ may be represented as $(2k+1)$, where $k$ is some integer
3. $n^2$ in this case is equal to $(2k+1)^{2}=4k^2+4k+1$
4. Simplify to $4(k^2+k)+1$
5. $4(k^{2}+k) | 2$ so $4(k^{2}+k)+1$ is odd
6. $n$ being not even implies $n^2$ being not even, therefore via De Morgans, $n^2$ being even implies $n$ being even