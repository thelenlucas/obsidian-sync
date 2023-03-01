---
tags: Computer_Science/Data_Structures
---

# Ghist
An [[Abstract Data Type]] used to acess information sequentially. Elements are stored as an array of class objects. Stores a current location that is used to `GetNext` and `ResetList`. 

# Functions

* `MakeEmpty()`
* `IsFull()`
* `GetLength()`
* `GetItem(ItemType item, bool &found)` - searches for item
* `PutItem()`
* `DeleteItem(Itemtype item)` - deletes item that matches
* `ResetList()`
* `GetNext()`

## DeleteItem
Two options for removing an item

1. Move all items up
2. Copy item to end of list to item location, as list is unordered

## MakeEmpty
Easy, just sets the length of the list to zero

## Resetlist
Sets operator to zero