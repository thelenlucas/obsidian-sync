---
tags: Mathematics/Discrete_Structures
---

# Ghist

One of the common [[Proof]] forms. The essentiality of this form is to prove that $P'\rightarrow Q$ is false, or it leads to a contradiction. If this is the case, $(P')'$, or $P$ is a [[Tautology]], and is thus true.

In other words, if we wish to prove $$P\rightarrow Q$$We may say prove by contradiction by attempting to show that $$P\wedge Q'$$is a contradiction. Thus $$(P\wedge Q' \rightarrow 0) \rightarrow (P\rightarrow Q)$$

# Example

Prove that $\sqrt 2$ is irrational:

1. Suppose not. In that case, $\sqrt 2 = \frac{a}{b}$, where $a$ and $b$ are intigers, and the fraction is in it's lowest term
2. Thus, $2 = \frac{a^2}{b^{2}}$
3. $2b^{2}= a^2$
4. Thus, $a^{2}$ is even, and so is $a$
5. $a=2k$ for some intiger $k$
6. $a^2=4k^2$ and $b^2=2k^2$
7. Thus $b$ is even, as $b^2$ are even
8. Since both items are even, the fraction is in it's lowest terms, and we have found a contradiction