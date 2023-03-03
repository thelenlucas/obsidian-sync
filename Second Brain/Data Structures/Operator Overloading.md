---
tags: Computer_Science/Data_Structures
---

# Ghist

In [[C++]], operators may be overloaded in order to change the function of a dattype

# Syntax

```C++
#include<iostream>
using namespace std;

class Complex {
private:
	int real, imag;
public:
	Complex(int r = 0, int i = 0) {real = r; imag = i;}
	
	// This is automatically called when '+' is used with
	// between two Complex objects
	Complex operator + (Complex const &obj) {
		Complex res;
		res.real = real + obj.real;
		res.imag = imag + obj.imag;
		return res;
	}
	void print() { cout << real << " + i" << imag << '\n'; }
};```

# Guidelines
 
1. At least one argument must be a class instance
2. Order may not be changed
3. Number of arguments may not be changed
4. Cannot add new operators