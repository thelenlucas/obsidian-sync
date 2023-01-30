---
tags: Computer_Science/Data_Structures
---

# Ghist

A linked list is a [[Data Structure]] that is created but not initialized at all times. Because of this, unlike [[C++ Arrays]], it may be manipulated with additions and subtractions.

# Structure

The linked list is made up of several components. The **Object** and the **Tail Pointer**. The object is some other data structure, such as a number, while the tail is a pointer to the next item in the list. The fist node is called the **Head**, and should never be lost, lest the whole list be destroyed.

# Example

```C++
struct node {
	int num;
	node* next_node;
}

int main {
	int some_number = 0;
	curr_node = node;
	node.num = some_number;
	node* head = &node;
	while (true) {
		n_node = node;
		n_node.num = some_num;
		curr_node.next_node = &n_node;
		curr_node = n_node;
	}
}
```

# Advantages/Disadvantages

Dynamically sized, and inserting elements is easy. However, there is no arbitrary acess to the linked list, meaning iteration must be performed to index it to any specific value, and especially only linear transversal is simple to impliment.

# Inserting Elements

To insert after some other element, all that must be done is the creation of a new node, pathing the old node to the new node, and pathing the new node to the next node. This naturally has special cases for the first and last positions.

# Deleting nodes

Deleting is easy, as long as you "close the gap" in the linked list's continuity. 