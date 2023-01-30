# Ghist
Functions have several different meanings, within both [[Mathematics]] and [[Computer Science]]. 

#Mathematics, #Computer_Science

# Mathematics
Withing [[Mathematics]], and especially [[Algebra]] and [[Calculus]], functions are isolated segments of math that have a unique output for every input. The function $f(x)$ will always output the same value of $f$ for every value of $x$. They are [[Deterministic]]

# Computer Science
In CS, functions are not nearly as [[Deterministic]]. They are not necessarily able to maintain output/input dichtonomy, and may return different values for identical inputs. They are instead usually vehicles for [[Abstraction]].

```Python
def printer(a):
	print(a)
```