---
tags: Computer_Science, Computer_Science/Rust
---

In [[Rust]], some types may be stored on the [[Stack]], and thus copying them is trivial, while other values do not impliment this behavior, such as [[Rust Strings]]. This is known as the *Copy* [[Trait]]. Several types impliment this by default:

-   All the integer types, such as `u32`.
-   The Boolean type, `bool`, with values `true` and `false`.
-   All the floating point types, such as `f64`.
-   The character type, `char`.
-   Tuples, if they only contain types that also implement `Copy`. For example, `(i32, i32)` implements `Copy`, but `(i32, String)` does not.