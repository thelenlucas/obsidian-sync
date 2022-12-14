---
tags: Computer_Science, Rust
---

In embedded rust, the entry point is the fucntion that the first processor starts executing when it is powered on. For the [[RP2040]], it is denoted as:

```Rust
#[rp2040_hal::entry]
fn main () -> ! {
	loop {}
}
```

(Note the [[Embedded Rust Processor Function]] requirements of no exit)