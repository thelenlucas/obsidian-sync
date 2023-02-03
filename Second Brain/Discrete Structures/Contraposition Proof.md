---
tags: Mathematics/Discrete_Structures
---

# Ghist

One of the many forms of [[Proof]], the contrapositive strategy attemts to establish a [[Propositional Logic]] via [[De Morgans]] theorem. That is, to prove $P \rightarrow Q$ via $Q' \rightarrow P'$.

# Example

Prove: For all ingagers $n$, if $n^2$ is even, then $n$ is even. 

Our original statement consisted of: If $n^2$ is even $\rightarrow$ $n$ is even. If we take the contropositive of this, we find: If $n$ is odd $\rightarrow$ $n^2$ is odd. If we can prove this, it will prove the original theorem as $$(Q'\rightarrow {P'}) \rightarrow (P\rightarrow Q)$$
Our proof is as follows:

1. Let $n$ be some arbitrary intiger so that $n$ is odd
2. Thus, $n = 2k + 1$ for some initiger $k$
3. $n^{2} = (2k+1)^{2}=4k^2+4k+1=2(2k^2+2k)+1$
4. $2(2k^2+2k)$ is even, and thus the addition of one makes it odd
5. Therefore $n^2$ is odd