---
tags: Computer_Science, Computer_Science/Rust
---

# Ghist

In [[Rust]], [[Variable]]s always follow several rules relating to their allocation and movement:

* Each [[Variable]] has an owner
* There may only be one owner at any given time
* When the owner goes out of [[Scope Rules]], the [[Variable]] is dropped