# calss_09

## Dunder Methods
These “dunders” or “special methods” in Python are also sometimes called “magic methods.” But using this terminology can make them seem more complicated than they really are—at the end of the day there’s nothing “magical” about them.
<br>
Dunder methods let you emulate the behavior of built-in types. For example, to get the length of a string you can call len('string'). But an empty class definition doesn’t support this behavior out of the box:
<img src='https://miro.medium.com/max/1200/0*2qlxUkQRsQdiM7MU.jpg'/>

### Special Methods and the Python Data Model
You can see Python’s data model as a powerful API you can interface with by implementing one or more dunder methods. If you want to write more Pythonic code, knowing how and when to use dunder methods is an important step.

### Enriching a Simple Account Class
Throughout this article I will enrich a simple Python class with various dunder methods to unlock the following language features:

* Initialization of new objects
* Object representation
* Enable iteration
* Operator overloading (comparison)
* Operator overloading (addition)
* Method invocation
* Context manager support (with statement)

<img src='https://miro.medium.com/max/1400/1*hyM-aAqna9iOWTHuWjq4-A.png'/>

* **Object Initialization: __init__** 
* **Object Representation: __str__, __repr__**
* **Iteration: __len__, __getitem__, __reversed__**
* **Operator Overloading for Comparing Accounts: __eq__, __lt__**
* **Operator Overloading for Merging Accounts: __add__**
* **Callable Python Objects: __call__**
* **Context Manager Support and the With Statement: __enter__, __exit__**

## Statistics in Python
#### Prerequisites:
Similar to the previous post, this article assumes no prior knowledge of statistics, but does require at least a general knowledge of Python and general data science worflows. 

#### What is probability?
he quintessential representation of probability is the humble coin toss. In a coin toss the only events that can happen are:

* Flipping a heads
* Flipping a tails



