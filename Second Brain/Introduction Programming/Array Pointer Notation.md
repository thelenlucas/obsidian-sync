---
tags: Computer_Science, Computer_Science/CPP
---
In [[C++]], arrays may be acessed as more than simple brackets ([]). Instead, they may also be accessed via a pointer operations. [[C++ Arrays]] are at their core, [[Pointer]]s to their data structure, so you can simply call:
```C++
float items = {0.0};
int index = 0;
float item = *(items + index);
```

This allows for [[Pointer Arithmatic]] operations