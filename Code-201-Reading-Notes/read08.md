# Layout
### Building Blocks : 
CSS treats each HTML element as if it is in its 
own box. This box will either be a block-level
box or an inline box.

### Containing Elements
If one block-level element sits inside another 
block-level element then the outer box is 
known as the containing or parent element.

### Controlling the Position of Elements
* **Normal flow**
* **Relative Positioning**
* **Absolute positioning**

#### box offset 
properties to tell the browser how far from the top or bottom 
and left or right it should be placed.

### psition tag
**static:**
I have not specified a width
property for the heading 
element


**Relative**: moves an 
element in relation to where it 
would have been in normal flow.

**fixed;** is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled.

**absolute;** is positioned relative to the nearest positioned ancestor

**sticky;** is positioned based on the user's scroll position.

### overlapping Elements
**z-index**: property specifies the stack order of an element

**float** : property specifies whether an element should float to the left, right, or not at all.

<img src='https://i0.wp.com/css-tricks.com/wp-content/uploads/2021/03/web-text-wrap.png?resize=540%2C270&ssl=1'>


**clear** :The clear property controls the flow next to floated elements.
The clear property specifies what should happen with the element that is next to a floating element.
 
 ### Screen Sizes
 Different visitors to your site will have different sized screens that show 
different amounts of information, so your design needs to be able to 
work on a range of different sized screens.

### Screen Resolution
Resolution refers to the number of dots a screen shows per inch. Some 
devices have a higher resolution than desktop computers and most 
operating systems allow users to adjust the resolution of their screens.

### Fixed Width Layouts
**advantages**:
* Pixel values are accurate at controlling size and positioning of elements.
* The size of an image will 
always remain the same 
relative to the rest of the 
page

**disadvantages** :
* You can end up with big gaps 
around the edge of a page
*  The page will often take up 
more vertical space than a 
liquid layout with the same 
content

### Liquid Layouts
**advantages**:
* Pages expand to fill the entire 
browser window so there are 
no spaces around the page 
on a large screen.
*The design is tolerant of 
users setting font sizes larger 
than the designer intended 

**disadvantages** :
* If the user has a very narrow 
window, words may be 
squashed and you can end up
* f the user has a wide 
window, lines of text can 
become very long

### Layout Grids
Composition in any visual art (such as design, painting, or photography) 
is the placement or arrangement of visual elements — how they are 
organized on a page. Many designers use a grid structure to help them 
position items on a page, and the same is true for web designers.

<img src = 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTxhp53CqyONIh1bSExGaCHYhjbCSjEmOnWJg&usqp=CAU'>
