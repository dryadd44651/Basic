# Linked List

![img](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2013/03/Linkedlist.png)

In simple words, a linked list consists of nodes where each node contains a data field and a reference(link) to the next node in the list.

```
class Node:
   def __init__(self, dataval=None):
      self.dataval = dataval
      self.nextval = None

class SLinkedList:
   def __init__(self):
      self.headval = None

list1 = SLinkedList()
```




## array vs linked list

Array: random access, fixed size

Arrays store elements in contiguous memory locations

linked list: traverse the node for acccess, dynamic link

Linked lists are less rigid in their storage structure and elements are usually not stored in contiguous locations

Linked lists offer some important advantages over other linear data structures. Unlike arrays, they are a dynamic data structure, resizable at run-time. Also, the insertion and deletion operations are efficient and easily implemented.


Implementation: stacks, queues, graphs

Example: Image viewer, Music Player 


### Time Complexity

SINGLY LINKED LIST OPERATION	  COMPLEXITY

Access i-th element	            O(N)

Traverse all elements	            O(N)

Insert element E at current point O(1)

Delete current element	        O(1)

Insert element E at front	        O(1)

Insert element E at end	        O(N)


Linked List is fundamental of tree and graphic


### Other linked list

Doubly Linked List (each node stores the address of previous node as well)
   Tip: add a tail in end of doubly linked list for O(1) to access tail
Circular Linked List (last node points to the first node)


https://www.geeksforgeeks.org/applications-of-linked-list-data-structure/
