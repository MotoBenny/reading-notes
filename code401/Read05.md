# Linked Lists and BigO

### [Big 0: Algoritm Efficiency](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/big_oh.html)

#big0 is used to describe the efficiency of an algorithm in terms of:
* ##### #Time, 
	* the ammount of time a function takes to complete, however time in this case refers the the number of steps the computer must take to complete the function, rather than the amount of seconds, minutes etc.
* ##### #Memory_space
	* Referse to the ammount of memory the function will use to store data and instructions.

BigO serves to describe the worst possible case of efficiency whe nan algorithm runs:
>	If we pass the largest ammount of data possible to this function, how long will it take to parse that data, and perform its opperation on all of it.
	
___

## [Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)

A sequence of nodes that or connected/linked to eachother. 
Importantly each node of a linked list refernces the next node.

### Terms:
 - #Linked_list - data structure of Nodes that link to the next node in the list
- #Singly - refers to the number of references to other nodes a single node has, A singly linked list's nodes only reference the next node in the list.
- #Doubly - doubly linked lists nodes, contain reference to the next and the previous nodes in the linked list
- #Node - Refers to the items in the linked list.
- #Next - this property of each node, contains the reference to the next node
- #Head - This is a reference to the first node in a linked list
- #Current - The Current is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list.
	
	## Traversing a linked list
	You are not able to use a foreach or a for loop to move within a linked list. Instead toy would access the 'Next' property of each node, to move along to the next item in the list.
	
	- The best way to traverse is with a `while` loop.