---
tags: Computer_Science
---

# Ghist

A byte pair encoder is a [[Data Compression]] algorithm that has found use in many [[Machine Learning]] applications.

# Algorithm

In BPC, repeated sequences of tokens are replaced by a token not in the dataset. For example, if we were to compress the string `AabBabBA`, we could reduce the string size by pairing down `ab` to `z` to get the string `AzBzBA`, which is shorter than the original string.