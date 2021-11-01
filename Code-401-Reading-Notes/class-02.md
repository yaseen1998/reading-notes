# class-02

## Unit tests and TDD?

Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.
<br>But Test-Driven Development is a strategy to think (and write!) tests first.

### AAA: Arrange, Act and Assert.
* Arrange: you need to organize the data needed to execute that piece of code (input);
* Act: here you will execute the code being tested (exercise the behaviour);
* Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

### The Cycle
** The cycle is made by three steps **:
* Write a unit test and make it fail
* Write the feature and make the test pass
*  Refactor the code — the first version doesn’t need to be the beautiful one

### TDD is not about the money/tests
TDD is how we can grow our software design consciously and well, just building what is needed to make the test pass.

### advantage of TDD : 
* craft the software design first
* Your code will be more reliable
* Beginning may be hard — and that’s fine

## What does the if __name__ == “__main__”: do?
it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 
<br>

### Why Do we need it?
if we want to use that module by importing we have to comment out our call. Rather than that approach best approach 

### Advantages : 
1- Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone
2- If you import this script as a module in another script,
3- Python files can act as either reusable modules
4- if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.

## Recursion
### What is Recursion? 
The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function.

### recursive function 
phenomenon is named as recursion and the function containing recursion

### How a particular problem is solved using recursion? 
terms of one or more smaller problems, and add one or more base conditions that stop the recursion

### Why Stack Overflow error occurs in recursion? 
If the base case is not reached or not defined, then the stack overflow problem may arise

### What is the difference between direct and indirect recursion? 
* direct recursive : if it calls the same function fun
* indirect recursive : if it calls another function say fun_new and fun_new calls fun directly or indirectly.

### What are the disadvantages of recursive programming over iterative programming? 
* written iteratively and vice versa is also true
* has greater space requirements than iterative program 
* has greater time requirements because of function calls and returns overhead

### What are the advantages of recursive programming over iterative programming? 
* clean and simple way to write code
*  We can write such codes also iteratively with the help of a stack data structure
* 



