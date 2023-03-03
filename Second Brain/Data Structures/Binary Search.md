---
tags: Computer_Science/Data_Structures
---

# Ghist

A search algorithm that allows for searching an [[Sorted List]] very easily

# Steps

1. Go to middle of list
2. If list item matches desired item, return
3. Otherwise, if item is less, move to lower half of split
4. Otherwise, move to upper half
5. Repeat until item found or no more spots to search

# Special Cases

## Linked Lists
We cannot use this here, as we cannot arbitrarliy access items