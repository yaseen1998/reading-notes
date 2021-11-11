# class-10

### What is a Stack
A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

#### Common terminology for a stack is
* push : put into the stack are pushed
<br>
always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.
* pop : removed from the stack are popped
<br>
Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.
* top : top of the stack
* peek : empty stack an exception will be raised.
<br>
When conducting a peek, you will only be inspecting the top Node of the stack.
* IsEmpty :  true when stack is empty 

<img src='https://www.tutorialandexample.com/wp-content/uploads/2020/12/Python-Stack-1.png'/>

##### FILO
First In Last Out
<br>
This means that the first item added in the stack will be the last item popped out of the stack.

##### LIFO
Last In First Out
<br>
This means that the last item added to the stack will be the first item popped out of the stack.

##### Stack Visualization

<img src='https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/stack1.PNG'/>

### What is a Queue
Common terminology for a queue is

* Enqueue - Nodes or items that are added to the queue.
* Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
* Front - This is the front/first Node of the queue.
* Rear - This is the rear/last Node of the queue.
* Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
* IsEmpty - returns true when queue is empty otherwise returns false.

#### Enqueue O(1)
When you add an item to a queue, you use the enqueue action. This is done with an O(1) operation in time because it does not matter how many other items live in the queue (n); it takes the same amount of time to perform the operation.
