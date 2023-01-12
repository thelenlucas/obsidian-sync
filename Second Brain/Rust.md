---
tags: Computer_Science, Computer_Science/Rust
---

# Ghist

Rust is a [[Statically-Typed]], [[Compiled]] [[Programming Language]] that is designed with several [[C Family]] concepts in mind, but attempts to fix some of the issues involved especially in [[C++]]. It has a much more powerful [[Compiler]], and a powerful system called the [[Borrow Checker]] that ensures [[Memory Safe]]ty, even without a [[Garbage Collector]].

# Ownership

In rust, ownership governs how rust manages memory. It's affirmed by the [[Borrow Checker]], which evaluates code on compile-time to avoid breaking rules. This allows easy allocation onto the [[Stack]] and the [[Heap]], without having to allocate and free memory manually.Variables always follow the [[Rust Owndership Rules]]