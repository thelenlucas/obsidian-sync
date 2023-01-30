---
tags: Computer_Science, Computer_Science/Rust
---

In [[Embedded Rust for the RP2040]], we have two seperate cores at our disposal. These may run code indipendantly and concurrently, and rust gives us the tools to run such code in a [[Memory Safe]] environment. However, when using embedded development, [[Embedded Rust Processor Function]]s may create issues in communications due to  the lack of a `return` function in processor functions. This, alongside stack allocation, are the main departure from the normal workflow.

# Stack Allocation

The first step in spinning up both cores in the allocation of the [[Stack]]. The first core (henceforth reffered to as CORE0), has it's stack automatically allocated thanks to the cortex-m-rt [[Crate]].

When spawning CORE1, in comparison, we need to allocate memory on the top of the stack manually. To put this into effect, the `.spawn()` function accepts a `usize` variable to denote it's section of the stack. We set this as a constant here with:

```Rust
static mut CORE1_STACK: Stack<4096> = Stack::new();
```

# Core Function

Just like the [[Entry Point]], CORE1 needs a function to begin executing, and just like the [[Embedded Rust Processor Function]] on the amin processor, it must never return. 

# Spawning the Core

First, we create a multicore object from our [[Peripheral Acess Crate]] and the [[Single Cycle IO Block]], then our core1 by indexing and slicing off the second index. We then can spawn our core's task. 

```Rust
let mut mc = Multicore::new(&mut pac.PSM, &mut pac.PPB, &mut sio.fifo);

let cores = mc.cores();

let core1 = &mut cores[1];

let _test = core1.spawn(unsafe { &mut CORE1_STACK.mem }, move || {
	core1_task(sys_freq)
});
```