#  OBJECT
Objects group together a set of variables and functions to create a model of a something you would recognize from the real world.


* IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES
* IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS 

<img src = 'https://cdn.programiz.com/sites/tutorial2program/files/javascript-object-properties.png'>

### object literal notation
way to create object in easist way

<img src = 'https://miro.medium.com/max/1838/1*KYFTHD69xtacnwbKRyFuqQ.png'>

### accessing an object 

<img src = 'https://dmitripavlutin.com/static/50a87420915de18f26da616865fe9825/05127/access-object-properties-2.png'>

# document Object model (DOM)
specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window. 

### THE DOM TREE
IS A MODEL OF A WEB PAGE As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.

#### the html dom tree of objects

<img src ='https://snipcademy.com/img/articles/javascript-document-object-model/dom.svg'>

### WORKING WITH THE DOM TREE
* **STEP 1:** ACCESS THE ELEMENTS
* **STEP 2:** WORK W ITH THOSE ELEMENTS 

### dom query
DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes.


**The getElementById()** method returns the element that has the ID attribute with the specified value.


**The querySelector()** method returns the first element that matches a specified CSS selector(s) in the document.
The querySelector() method only returns the first element that matches the specified selectors. To return all the matches, use the querySelectorAll() method instead.


**The getElementsByClassName()** method returns a collection of all elements in the document with the specified class name, as an HTMLCollection object.


**The getElementsByTagName()** method returns a collection of all elements in the document with the specified tag name, as an HTMLCollection object.


**The querySelectorAll()** method returns all elements in the document that matches a specified CSS selector(s), as a static NodeList object.


### select element from a nodelist:
 **1-item() method** :which will return an individual node from the Node list.
