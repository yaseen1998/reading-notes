# Read: Class 10
## What is a ‘call’?
The call stack is primarily used for function invocation (call)
. Since the call stack is single, function(s) execution, is done,
one at a time, from top to bottom. It means the call stack is synchronous.

## How many ‘calls’ can happen at once?
 Since the call stack is single, function(s) execution, is done, one at a time, 
 from top to bottom. It means the call stack is synchronous.
 
## What does LIFO mean?
 First Out (LIFO) principle to temporarily store and manage function invocation (call).
 <br>  it means that the last function that gets
 pushed into the stack is the first to be pop out, when the function returns.
 
 ## Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
 
 <img src = 'https://i.stack.imgur.com/w19l1.png'>
 
 ## What causes a Stack Overflow?
 A stack overflow occurs when there is a recursive function (a function that calls itself)
 without an exit point. The browser (hosting environment) has a maximum stack 
 call that it can accomodate before throwing a stack error.
 
 ## What is a ‘refrence error’?
 This is as simple as when you try to use a variable that is not yet declared you get this type os errors.
 
 ## What is a ‘syntax error’?
is occurs when you have something that cannot be parsed in terms of syntax, 
like when you try to parse an invalid object using JSON.parse.

## What is a ‘range error’?
object indicates an error when a value is not in the set or range of allowed values

## What is a ‘tyep error’?
this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible,
like accessing a property in an undefined type of variable.

## What is a breakpoint?
The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.

## What does the word ‘debugger’ do in your code?
just show the result for your code




