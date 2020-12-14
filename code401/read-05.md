# Reading Assignment 05
*Read*:
- [Linked List - Code Fellows](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)
- [Linked List Pt 1 - Medium](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)
- [Linked List Pt 2 - Medium](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)

### Linked Lists
A linked list is a linear but dynamic data structure made up of elements called *nodes*. Nodes only contain their value and a reference to the following node. A linked lists starting point is always at the head, and the last node in the list will have it's next pointing to NULL. Technically, this is a *singly linked list*. 

A *doubly linked list* has the same rules applied except every node also keeps track of it's other neighbor; the previous node to it. 

However, there is an exception to the last node in the linked list pointing to NULL. This only happens when building a *circular linked list*.  A circular linked list keeps track of both a head and tail reference, where the head is the first node in the list and the tail is the last node in the list, but is still pointing to the first node. 

Unlike arrays, a linked list cannot be traversed using for or forEach. Every element in the list has very limited knowledge about the rest of the list. Traversal through a linked list is dependent on what the node's next reference is. 



