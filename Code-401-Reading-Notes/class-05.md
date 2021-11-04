# class-04

## Big O: Analysis of Algorithm Efficiency
 is used to describe the efficiency of an algorithm or function.
 <br> 
  describe the Worst Case of efficiency an algorithm can have in performing it’s job. It specifically looks at the factors mentioned above
 ** based on 2 factors: ** :
 * Runnning Time ( time complexity) : The amount of time a function needs to complete.
 * memory space (space complexity) : The amount of memory resources a function uses to store data and instructions.

#### what the key area for space and time : 
* Input Size
* Units of Measurement
* Orders of Growth
* Best Case, Worst Case, and Average Case

## Linked Lists
What is a Linked List A Linked List is a sequence of Nodes that are connected/linked to each other

## Tremminology : 
* Linked List - A data structure that contains nodes that links/points to the next node in the list.
* Singly - Singly refers to the number of references the node has. 
* Doubly - Doubly refers to there being two (double) references within the node.
* Node - Nodes are the individual items/links that live in a linked list. 
* Next - Each node contains a property called Next. 
* Head - The Head is a reference of type Node to the first node in a linked list.
* Current - The Current is a reference of type Node to the node that is currently being looked at.

### Singly Linked Lis
<img src='https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2013/03/Linkedlist_insert_middle.png'/>

## Traversal
When traversing a linked list, you are not able to use a foreach or for loop. We depend on the Next value in each node to guide us where the next reference is pointing. The Next property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.

 ### Adding a Node
 we have to replace the current Head of the linked list with the new node, without losing the reference to the next node in the list.
 
 ### Print Out Nodes
 printing out all of the nodes in a Linked List is very similar to what we did in the Includes() method. This is because we are leveraging our Current node and a while loop to traverse through the existing linked list.
 
