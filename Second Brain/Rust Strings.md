---
tags: Computer_Science, Computer_Science/Rust
---

# Ghist

In [[Rust]], [[String]] data types are either stored as one of two options. [[String Literal]]s or with `String::` notation.

# String Literals

Follow [[String Literal]] rules in that they are hardcoded, and may not be changed. They are for all intents and purposes, [[Constant]]s.

# Rust Strings

Rust strings are a compound data type that consist of a pointer, a length, and a capacity. Notably, performing
```Rust
fn main() {
	let s = String::from("hello");
	let a = s;
}
```

Will not copy `s` into `a`, it will provide a new string object that has identical length and capacity as `s`, and provides a [[Pointer]] to `s`.

As a consequence of this, after this operation, `s` is no longer considered valid by the compiler, as an attempt to avoid memory corruption caused by double freeing a memory slot. Overall, it functions much like [[Shallow Vs. Deep Copy]] does. There is a method `String::clone()` that will clone a string down to the bye, which is naturally more computationally expensive. Note that since vairables are freed from the heap after they leave scope, code such as:

```Rust
fn main() {
	let s = String::from("Hello");
	take_owner(s);
	let a = s.copy();
}

fn take_owner(something: String) {
	println!("{}", something);
}
```

Would throw a compile-time error, as `s` is no longer valid, having its assosiated heap space freed at the end of `take_owner()`. This can be avoided by having a [[Function]] process and then return a value, but it's easier to use Rust's [[Borrow]] system instead.