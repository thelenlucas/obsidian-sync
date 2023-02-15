---
tags: Mathematics/Discrete_Structures
---

# Ghist

In [[Formal Logic]], an item is a predicate [[WFF]] when it uses [[Quantifier]]s and takes a valid form using [[Predicate Verb]]s

# Examples

1. $P(x)\wedge Q(y)$
2. $(\forall x)[P(x)\rightarrow Q(x)]$
3. $(\forall x)((\exists y)[P(x,y) \wedge Q(x,y)]\rightarrow R(x))$

# Syntax
## Scope
Brackets and parens imply the the scope of the quantifier, similar to the scope of a function in computer science. 

## Free Variables
Free variables are varialbes without a quantifier for a given scope. We may not determine the truth value of a string with free variables, unless disjunctions may apply.