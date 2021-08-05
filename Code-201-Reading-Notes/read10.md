# error handling & debugging
### order of execution 
 some tasks cannot complete until another statement or function has been run: 
 
 
 The JavaScript interpreter uses the concept of execution contexts. 
There is one global execution context; plus, each function creates a new 
new execution context. They correspond to variable scope.

### execution context 
* GLOBAL CONTEXT 
* FUNCTION CONTEX
* FUNCTION CONTEX

### variable scope 
* GLOBAL SCOPE
* function level scope

### the stack
the javascript interpreter processcs one line of code at a time when a statement needs data from another function it stacks the new function ontop of the current task


### EXECUTION CONTEXT & HOISTING
1: PREPARE 
* The new scope is created 
* Variables, functions, and arguments are created 
* The value of the this keyword is determined

2: EXECUTE 
* Now it can assign values to variables 
* Reference functions and run their code 
* Execute statements

### UNDERSTANDING ERRORS
If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handl ing code.

### ERROR OBJECTS
Error objects can help you find where your mistakes are and browsers have tools to help you read them.

<img src = "https://tecadmin.net/wp-content/uploads/2015/08/jquery-object-error.png">

#### Syntax Error 
This is caused by incorrect use of the rules of the language <br>
1- MISMATCHING OR UNCLOSED QUOTES <br>
2-MISSING CLOSING BRACKET <br>
3-MISSING COMMA IN ARRAY <br>
4-MALFORMED PROPERTY NAMe

#### Ref erenceError
VARIABLE DOES NOT EXIST This is caused by a variable that is not declared or is out of scope.<br>
1-VA RIABLE IS UNDECLARED <br>
2-NAMED FUNCTION IS UNDEFINED 

#### Eval Error
the eval() function evaluates text through the interpreter and runs it as code

#### url error
If these characters are not escaped in URls, they will cause an error: / ? & I : ;

#### type error 
This is often caused by trying to use an object or method that does not exist.<br>
1-INCORRECT CASE FOR document OBJECT <br>
2-INCORRECT CASE FOR write() METHOD <br>
3-METHOD DOES NOT EXIST<br>
4-DOM NODE DOES NOT EXIST<br>

#### range error
If you call a function using numbers outside of its accepted range.<br>
1-CANNOT CREATE ARRAY WITH -1 ITEMS <br>
2-NUMBER OF DIGITS AFTER DECIMAL IN tofixed() CAN ONLY BE 0-20 <br>
3-NUMBER OF DIGITS IN toPrecision() CAN ONLY BE 1-21 <br>

#### error
GENERIC ERROR OBJECT<br>
The generic Error object is the template (or prototype) from which all other error objects are created.

#### nan
NOT AN ERROR <br>
Note: If you perform a mathematical operation using a value that is not a number, you end up with the value of NaN, not a type error.

### HOW TO DEAL WITH ERRORS 
* **1: DEBUG THE SCRIPT TO FIX ERRORS**
* **2: HANDLE ERRORS GRACEFULLY**

### A DEBUGGING WORKFLOW
Debugging is about deduction: eliminating potential causes of an error. Here is a workflow for techniques you will meet over the next 20 pages. Try to narrow down where the problem might be, then look for clues. 
<br>
#### WHERE IS THE PROBLEM? 
First, should try to can narrow down the area where the problem seems to be.<br>
1-Look at the error message<br>
2- Look at the error message<br>
3-Use breakpoints where things are going wrong. <br>

#### WHAT EXACTLY IS THE PROBLEM? 
Once you think that you might know the rough area in which your problem is located<br>
1- When you have set breakpoints, you can see if the variables around them have the values you would expect them to.<br>
2-Break down I break out parts of the code to test smaller pieces of the functionality. <br>
3-  Check the number of parameters for a function, or the number of items in an array. <br>


### LOGGING DATA TO THE CONSOLE 
* console.log() method.
* conso1e.info() can be used for general information
* console.warn() can be used for warnings
*  console.error() can be used to hold errors 


### BREAKPOINTS
You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time.<br>


















