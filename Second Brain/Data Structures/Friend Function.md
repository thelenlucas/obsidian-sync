---
tags: Computer_Science/Data_Structures
---

# Ghist

In [[C++]], friend functions are [[Computer Science Theory/Function]]s that is not a class member, but can acess private data fields. The prototypes for these functions appear only in the class definition.

# Syntax

```C++
class Distance {
	private:
		int meter;
		friend int addFive(Distance);
}

int addFive(Distance d) {
	//Private accessed
	d.meter += 5;
	return d.meter;
}
```

# Advantages

Allows for more effecient code, allows sharing of private class members, and allows for additional functionality not in the base classallocations.