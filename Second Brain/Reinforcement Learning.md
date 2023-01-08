---
tags: Computer_Science/Machine_Learning
---

Reinforcement learning is a form of [[Machine Learning]] that can be applied to many algorithms, in which an agent randomly changes paramaters, and then gathers information on statistcal changes, before repeating hte cycle based off of that knowledge. It is usally modeled as

* A set of states $S$
* A set of actions $A$
* The probability of changing from action $s$ to action $s'$ after taking action $a$ $P_{a}(s,s')$
* The reward after transitioning from $s$ to $s'$ via $a$ $R_{a}(s,s')$

This is known as a [[Markov]] decision process. 