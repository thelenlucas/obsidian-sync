---
tags: Mathematics/Linear_Algebra
---

# Ghist

In [[Linear Algebra]], a Vector space is a [[Set]] for which it's components can act as [[Vector]]s. 

# Definition

A vector space is a non-empty [[Set]] of values for which several axioms hold true for all $u,w,v$ inside the space $V$, and all scalars $c,d$:

1. $u+v$ is in $V$
2. $u+v=v+u$
3. $(u+v)+w=u+(v+w)$
4. There exists some vector $0$, so that $u+0=u$
5. For every $u$, there is some vector $-u$ so that $u+(-u)=0$
6. $cu$ is in $V$
7. $c(u+v)=cu+cv$
8. $(c+d)u=cu+du$
9. $(cd)u=c(du)$
10. $1u=u$

# Subspaces

A [[Vector Space]] can have a sub-set of another vector space. If it qualifies, it is thus called a [[Subspace]]. Subspaces must qualify in several axioms, for the subspace $H$ of $V$:

1. The [[Zero Vector]] of $V$ is in $H$
2. For every $u$ and $v$ in $H$, $u+v$ is in $H$ (Closed under vector addition)
3. For each $u$ in $H$ and each scalar value $c$, $cu$ is in $H$ ([[Closure Under Multiplication]])
