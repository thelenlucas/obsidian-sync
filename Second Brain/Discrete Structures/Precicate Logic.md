---
tags: Mathematics/Discrete_Structures
---

# Ghist

Predicate logic takes the form of conjuncted [[Predicate String]]s. Like [[Propositional Logic]], predicate logic statements much be intrinstically true to be valid, or true in all situations.

The [[Propositional Logic]] inference and equivilance rules are still in effect - we can still use items like modus poens and the like.

# Important Inference Rules

| From                                            | Can Derive                                               | Rule                               | Restrictions                                                                                                        |
| ----------------------------------------------- | -------------------------------------------------------- | ---------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| $(\forall x)P(x)$                               | $P(t)$ where $t$ is a variable or constant symbol        | [[Universal Instantiation]]  - ui  | If $t$ is a variable, it must not be within the scope for which $t$ has a [[Quantifier]]                            |
| $(\exists x)P(x)$                               | $P(a)$ where $a$ is a constant symbol not previosly used | [[Existential Instantiation]] - ei | Must be the first rule that introduces $a$                                                                          |
| $P(x)$                                          | $(\forall x)P(x)$                                        | Universal Generalization - ug      | $P(x)$ has not been deduced from either a statement where $x$ is a free variable nor from a free variable use of ei |
| $P(x)$ or $P(a)$ where $a$ is a constant symbol | $(\exists x)P(x)$                                        | Existential Generalization - eg    | To go from $P(a)$ to its derivation, $x$ must not appear in $P(a)$                                                  |

## Examples

#### Universal Instantiation
The statement "All Humans are mortal, and socratese is a human, therefore socratese is mortal" may be encoded in predicate logic. Here $H(x)$ is a [[Predicate Verb]] that states $x$ is human, $s$ is a constant symbol (socratese), and $M(x)$ is mortal:$$(\forall x)[H(x)\rightarrow M(x)]\wedge H(s) \rightarrow M(s)$$We can prove this using our tools of [[Formal Logic]]:

1. $(\forall x)[H(x)\rightarrow M(x)]$ - hyp
2. $H(s)$ - hyp
3. $H(s)\rightarrow M(s)$ - 1, ui
4. $M(s)$ - 2, 3, mp

#### Existential instantiation
The [[Existential Instantiation]] power allows us to create new constant symbols, but not to assume anything about them, thus:

1. $(\forall x)[P(x) \rightarrow Q(x)]$ - hyp
2. $(\exists y)P(y)$ - hyp
3. $P(a)$ - 2, ei
4. $P(a) \rightarrow Q(a)$ - 1, ui
5. $Q(a)$ - 3, 4, mp

In step 3, we named $a$ as some item with property $P(a)$. We then can utilize this to claim that $Q(a)$ is implied, as step one claims that this is true for all objects in the domain.

#### Universal Generalization
We may prove $$(\forall x)[P(x)\rightarrow Q(x)]\wedge (\forall x)P(x) \rightarrow(\forall x)Q(x)$$In order to do so, we take the steps:

1. $(\forall x)[P(x)\rightarrow Q(x)]$ - hyp
2. $(\forall x)P(x)$ - hyp
3. $P(x) \rightarrow Q(x)$ - 1, ui
4. $P(x)$ - 2, ui
5. $Q(x)$ - 4, 3, mp
6. $(\forall x)Q(x)$ - 5, ug

#### Existential Generalization
Existential generalization is fairly strange, but in essense, it allows us to say that if an object has been named as a property, there exists some object with that property.

1. $(\forall x)P(x)$ - hyp
2. $P(x)$ - 1, ui
3. $(\exists x)P(x)$

