# class-04
## Classes and Objects
Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

<img src='https://miro.medium.com/max/1400/1*9xf-4NoyRIeCGN6hZPkYJw.png'/>

### Accessing Object Variables & function
key = nameofclass
key.keyinclass

You can create multiple different objects that are of the same class(have the same variables and functions defined). However, each object contains independent copies of the variables defined in the class. For instance, if we were to define another object with the "MyClass" class and then change the string in the variable above:

## Thinking Recursively in Python
<img src='https://robocrop.realpython.net/?url=https%3A//files.realpython.com/media/elves_7.8d1af1cd85c8.png&w=1918&sig=24bad525e070e8248cc8fcce28fc3f52c68a69f9'/>

### Recursive Functions in Python

A recursive function is a function defined in terms of itself via self-referential expressions.
<br>
This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. 

### Maintaining State
maintain state during recursion you have to either:
* Thread the state through each recursive call so that the current state is part of the current call’s execution context
* Keep the state in global scope

### Recursive Data Structures in Python
A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure

### Naive Recursion is Naive
Naively following the recursive deﬁnition of the nth Fibonacci number was rather inefficient

## Python Testing with pytest: Fixtures and Coverage
. pytest has become quite popular, in no small part because it's so easy to write tests and integrate those tests into your software development process. I've become a big fan, mostly because after years of saying I should get better about testing my software, pytest finally has made it possible.

### Coverage
This is all great, but if you've ever done any testing, you know there's always the question of how thoroughly you have tested your code. After all, let's say you've written five functions, and that you've written tests for all of them

### Summary
If you haven't guessed from my three-part focus on pytest, I've been bowled over by the way this testing system has been designed. After years of hanging my head in shame when talking about testing, I've started to incorporate it into my code, including in my online "Weekly Python Exercise" course. If I can get into testing, so can you. And although I haven't covered everything pytest offers, you now should have a good sense of what it is and how to start using it.
