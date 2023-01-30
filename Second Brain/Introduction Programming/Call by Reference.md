Calling by reference in [[C++]] is a tecnique that allows ofr the breaking of [[Scope Rules]]. When a value is passed into a [[Function]] as 
```C++
void add(float &x, float &y) {
	//...
}
```
MOdifying either of these values modifies their passed in values, contrasting [[Call By Value]], which makes a copy of these values when passed
