# table
A table represents information in a grid format.

### Basic Table Structure
* table tag :used to create table
* tr tag : indicate to start of each row using the opening
* td tag : represented each cell of a atable
* th tag : represent the heading for either column or a row

<img src = 'https://gocoding.org/wp-content/uploads/2020/06/HTML-Table-Syntax.png'>

you can use (colspan="2"   or rowsoan="2") with td or th tag to spanning row or spanning column


### Long Tables
There are three elements that help distinguish between the main content of the table and the first and last rows <br> 
These elements help people who use screen readers and also allow you to style these sections in a different manner than the rest of the table 

* thead tag : The headings of the table should sit inside the thead tag
* tbody tag : The body should sit inside the tbody tag element.
* tfoot tag : The body should sit inside the tbody tag element.

### CSS element for table
* width
* cellpadiing
* cellspacing
* border
* bgcolor

# constructor notation
we are creating the same objest we created in literal notation above, by calling the constructor function with the “new” keyword.
<img src = 'https://csawesome.runestone.academy/runestone/books/published/csawesome/_images/worldConstructors.png'>

#### updating an object 
**1-object.propertn mame = property value**
**2-object[propertn mame] =  property value**

### CREATING OBJECTS USING CONSTRUCTOR SYNTAX


<img src ='https://miro.medium.com/max/1400/1*TF3BiUEOt9DPOPJkqas53g.png'>

function Hotel(name, rooms, booked) { <br>
this.name = name; <br>
th is.rooms = rooms; <br>
this.booked = booked; <br>
this.checkAvailability = function() <br>
return this.rooms - this.booked; <br>
} ; <br>
var quayHotel =new Hotel('Quay', 40 , 25);<br> 
var parkHotel =new Hotel('Park', 120, 77);<br>

### A KEYWORD
The keyword this is commonly used inside functions and objects. 
Where the function is declared alters what this means. It always refers 
to one object, usually the object in which the function operates. 
* **global variables**
* **METHOD OF AN OBJECT**

### RECAP: STORING DATA 
In JavaScript, data is represented using name/value pairs. To organize your data, you can use an array or object to group a set of related values. In arrays and objects the name is also known as a key.

* VARIABLES
* arrays
* individual objects
* muliple objects

