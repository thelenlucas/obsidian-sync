---
tags: Computer_Science, Computer_Science/Rust
---

# Ghist

In [[Rust]], whether or not a [[Variable]] may be assigned on the [[Stack]] or the [[Heap]] depends on their size. Items of a known size, such as [[Integer]]s or [[Float]]s, may be quickly pushed onto the stack. Data types with unkown sizes, such [[String]]s, have less known types, and may not easily allocated onto the [[Stack]].