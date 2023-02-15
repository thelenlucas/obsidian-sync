---
tags: Mathematics/Discrete_Structures
---

# Ghist

In [[Propositional Logic]], a statment is some scentence that is either true or false, without any inditermanents.

# Examples

## Of propositions
1. Ten is less than seven
2. Cheyenne is the Capital of Wyoming
3. There are life forms on other planets

## Not propositions
4. She is very Talented

Statments 1 and 2 are [[Proposition]] [[WFF]]s because they are false and true, respecively. Scentence 3 is a proposition because it is either true or false, it is determined, though we do not know it's value. 4 is not a proposition because it is neither true or false, since "she" is not specified.

# Connectives

The qualities of a proposition are held together via connectives that determine the relationship between the different subunits of a proposition:

1. Conjunctive (AND)
2. Disjunctive (OR)
3. Implication (->)
4. Equivilance ( < - > )
5. Negation (')

## Special note on negation

Negating a conjunction, disjunction or implication "reverses" that connection from a C to a D and vice versa, and changes the direction of the implication.

# Arguments

Propositional Arguments are represented by statements of Conjunctions terminating in some conclusion:$$P_{1}\wedge P_2\wedge\cdot\cdot\cdot\wedge P_{n}\rightarrow Q$$The goal of propositional logic is often to determine the validity of these arguments.

## Validity

Propositional Arguments are valid when they logicalally follow from their hypotheses to their conclusions. Valid arguments should attempt to be intrisically true. That is, they should be [[Tautology]]s.

## Example

*Consider the following argument. If George Washington was the first president of the United States, then John Adams was the first vice president. George Washington was the first president of the United States. Therefore John Adams was the first vice president.*

If we allocate $G$ and $J$ to the validity of their respective statements, this argument would take the form of $$(G\rightarrow J)\wedge(G)\rightarrow J$$This argument is intrinsically true if we take the validity of it's hypotheses to be true.