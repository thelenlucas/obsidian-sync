---
tags: Mathematics/Discrete_Structures
---

# Ghist

The first principle of [[Logical Induction]] broadly states that for some assertion $P(x)$, if:

1. $P(1)$ is true
2. $(\forall k)[P(k) \text{true} \rightarrow P(k+1) \text{true}]$

Then $P(n)$ is true for all positive intigers $n \ge 1$.

# Example

Prove that $$1+3+5+\cdot\cdot\cdot+(2n-1)=n^2$$First, we establish the base case$$P(1)=1^2$$Which is true. Then we assume that the case for $P(n)$ is true$$1+3+5+\cdot\cdot\cdot+(2n-1)=n^2$$Now, we attempt to show that $$P(n)+(2(n+1)-1)=P(n+1)$$Which would imply that $P(n)$ being true -> $P(n+1)$ being true.

1. $1+3+5+\cdot\cdot\cdot+(2n-1)+(2(n+1)-1)=(n+1)^2$
2. $n^{2}+(2(n+1)-1)=(n+1)^{2}$
3. $n^2+2n+1=$
4. $(n+1)^2=(n+1)^2$

This proves via induction.