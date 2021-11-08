# class-07
## Python Scope & the LEGB Rule: Resolving Names in Your Code
the scope of a name defines the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on.
<br>
two general scopes:
* Global scope: The names that you define in this scope are available to all your code.
* Local scope: The names that you define in this scope are only available or visible to the code within the scope
<br>
Some languages like Python use scope to avoid this kind of problem. When you use a language that implements scope, there’s no way for you to access all the variables in a program at all locations in that program. In this case,
If you can’t access the name, then you’ll say that the name is out of scope.

## Names and Scopes in Python
Python uses the location of the name assignment or definition to associate it with a particular scope. In other words, 
<br>
### Python Scope vs Namespace
the concept of scope is closely related to the concept of the namespace. As you’ve learned so far, a Python scope determines where in your program a name is visible. Python scopes are implemented as dictionaries that map names to objects. These dictionaries are commonly called namespaces. These are the concrete mechanisms that Python uses to store names. They’re stored in a special attribute called .__dict__.
<img src='https://i.ytimg.com/vi/R2_beoINHe4/maxresdefault.jpg'/>

### Using the LEGB Rule for Python Scope
Python resolves names using the so-called LEGB rule, which is named after the Python scope for names.
* Local (or function) scope is the code block or body of any Python function or lambda expression. 
* Enclosing (or nonlocal) scope is a special scope that only exists for nested functions. 
* Global (or module) scope is the top-most scope in a Python program, script, or module.
* Built-in scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session.

## Don't be CONFUSED by BIG O notation anymore!
big O rules:
* different steps get added
if a bit of code big O for it O(n) the next bit = O(b) so total big O=O(n+b)

* drop constant

* use different variables for different inputs
if array1 of size a if array2 of size b loop through each array so big O total= O(a*b) not O(n^2)

* drop non-dominate terms
if a bit of code big O for it O(n) the next bit = O(n^2) so total big O=O(n+n^2)=O(n^2)
