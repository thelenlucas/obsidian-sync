# Ghist
In the [[C Family]] and other [[Programming Language]]s, pointers are a datatype that "points to" the [[Memory Adress]] of another variable. These have several uses, but the main ones include modification of out-of-scope memory and the saving of memory across different scopes.

Part of a series within #CS121

# The Code
Pointer variables are denoted by the operator ```*``` ([[C Family * Operator]]) For example

```C++
int* pointerVar;
```

Denotes a pointer to an integer named ```pointerVar```. We can assign these using the [[Reference Operator]] `&`. If we were to perform

```C++
int num = 4;
int* ptr = &num;
```

We would obtain a variable pointing towards `num`, that we could later dereference to acess `num` out of scope. We do this once again using the `*` operator, [[C Family * Operator]]

```C++
//This segment creates a variable, adds a pointer to its location
//and then uses that pointer to add 1 to the original float
float sum = 0.5;
float* sumPointer = &sum;
float s = *sumPointer;
s++;
cout << sum;
```