---
tags: Mathematics/Discrete_Structures
---

# Ghist

In [[Discrete Mathematics]], a recursive definition is one that relies on itself in a previous iteration to determine it's current value. One of the most popular recursively defined functions is the Fibbonacci Sequence:

1. $F(1)=1$
2. $F(2)=1$
3. $F(n)=F(n-1)+F(n-2)\text{ for } n\gt 2$

This has several interesting properties, such as approaching the golden ratio.

# Proving

We can use these recursive definitions to prove interesting items about these relations, but more generally helpful is usually using [[Logical Induction]] to assist in finding general solutions when applicable.

#### Prove that $F(n+4)=3F(n+2)-F(n) \text{ for all } n\ge 1$
The base step here is:

1. $F(1+4)=3F(1+2)-F(1)$
2. $F(5)=3F(3)-F(1)$
3. $5=3(2)-1$

and

1. $F(6)=3F(4)-F(2)$
2. $8=3(3)-1$

Now we assume that for all $r$, $1\le r \le k$, $F(r+4)=3F(r+2)-F(r)$.

Now we much show that this holds for $k+1$, where $k\ge 3$. Thus$$F(k+1+4)=3F(k+1+2)-F(k+1)$$We can then substitute down using the original reccurance relation $F(r+4)=3F(r+2)-F(r)$ that we determined earlier, with $r=k-1,k+1$, as well as the original recurrance relation:

1. $F(k+5)=F(k+3)+F(k+4)$
2. $=[3F(k+1)-F(k-1)]+[3F(k+2)-F(k)]$
3. $=3[F(k+1)+F(k+2)]-[F(k)+F(k-1)]$
4. $=3[F(k+3)]-F(k+1)$

Thus we have proven via the [[Second Principle of Induction]].

