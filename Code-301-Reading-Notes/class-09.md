# Read: Class 09
 
 ## What is functional programming?
 is a programming paradigm — a style of building the structure and elements 
 of computer programs — that treats computation as the evaluation of 
 mathematical functions and avoids changing-state and mutable data 
 
 ## What is a pure function and how do we know if something is a pure function?
 * It returns the same result if given the same arguments (it is also referred as deterministic)
 * It does not cause any observable side effects
 * Reading Files
 * Random number generation

 ## What are the benefits of a pure function?
 * The code’s definitely easier to test
 * We don’t need to mock anything
 * we can unit test pure functions with different contexts
 
 ## What is immutability?
 its state cannot change after it’s created.
 If you want to change an immutable object, you can’t.
 Instead, you create a new object with the new value.
 
 ## What is Referential transparency?
 Basically, if a function consistently yields the same result for the same input, 
 it is referentially transparent.
<br> `pure functions + immutable data = referential transparency`
 
 ## What is a module?
 Each module in Node.js has its own context, 
 so it cannot interfere with other modules or pollute global scope.
 Also, each module can be placed in a separate
 
## What does the word ‘require’ do?
 Node.js follows the CommonJS module system, 
 and the builtin require function is the easiest way to include 
 modules that exist in separate files
 
 ## What do we have to do to make a module available?
  In this scope, we use the module.exports object to expose modules, 
  and require to import them.
 
 
 
 
 
 
 
 
 
 
 
 
 
 
