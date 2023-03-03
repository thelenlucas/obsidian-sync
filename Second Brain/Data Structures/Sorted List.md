---
tags: Computer_Science/Data_Structures
---

# Ghist

It is garunteed that the item in `i` is less than or equal to the item in `i+1`

# Operations

* Create a new list 
* Empty an existing list
* Add an item to the list (if unsorted)
* Add an item to the list (if sorted)
* Delete an item from the list
* Find an item in the list
* Determine the length of the list
* Determine if the list is empty
* Determine if the list is full
* Iterate through the list

# Differences from [[Unsorted List]]

* We guarentee list elements are sorted
* This requires changing our transformer functions

## PutItem

1. Find where item should be placed in list
2. Create space for element
3. Insert item in spot

The list is already sorted, so a simple linear search may be used. Space is created by moving all below elements down one space.

## DeleteItem

1. Find item to delete
2. Delete item
3. Move all other items up

