# Html Text
#### heading tag 
heading text has six level start from 1 to 6
![heading](https://seranking.com/blog/wp-content/uploads/2019/08/Diagrammatic-Representation-of-Heading-Tag-Hierarchy.png)

#### paragraphs tag 
To create a paragraph, surround the words that make up the paragraph with an opening <'p'> tag and closing <'/p'> tag.

#### Bold & Italic
<'b'> : can make characters appear bold.

<'i'> : can make characters appear italic.

#### Superscript & Subscrip
<'sup'> : appears half a character above the normal line

<'sub'> :  appears half a character under the normal line

### Line Break 
<'br /'> : inserts a single line break.

<'hr /'> : displayed as a horizontal rule that is used to separate content

## Semantic Markup
text elements that are not intended to affect thestructure of your web pages, but they do add extra information to the pages

* <'strong'> :  indicates that its content has strong importance.
* <'em'> :  indicates emphasis that subtly changes the meaning of a sentence.

* <'blockquote'> :  tag specifies a section that is quoted from another source.
* <'q'> : defines a short quotation , Browsers normally insert quotation marks around the quotation.
* <'abbr'> : tag defines an abbreviation or an acronym
* <'cite'> : tag defines the title of a creative work
* <'dfn'> : tag stands for the "definition element"
* <'address'> :  tag defines the contact information for the author/owner of a document or an article.
* <'ins'> & <'del'> : The <'ins'> element can be usedto show content that has been inserted into a document, while the <'del'> element can show text that has been deleted from it.

* <'s'> : indicates something that is no longer accurate or relevant

# Introducing CSS
CSS allows you to create rules that specify how the content of an element should appear . 

CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.
![ selector and a declaration](https://studentweb.elgin.edu/academic/jbrzezinski7797/CIS%20148/css-syntax.gif)

### External CSS
![external](https://way2tutorial.com/images/external_sheet.png)
<'link> :  tell the browser where to find the CSS file used to style the page. 

type : attribute specifies the type of document being linked to

href : This specifies the path to the CSS file 

rel : This specifies the relationship between the HTML page and the file it is linked to

### Internal CSS
![internal](https://way2tutorial.com/images/internal_sheet.png)

<'style'> : should use the type attribute to indicate that the styles are specified in CSS.

### CSS Selectors 
In CSS, selectors are patterns used to select the element(s) you want to style.
<img src = 'https://pbs.twimg.com/media/EdTVA1CWAAAvVIu.jpg:large' >

# Basic Javascript Instructions
#### statement
A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step   

#### comment
* multi-line :  starting with the (/+star) characters and ending with the (star+/) characters.

* single-line : anything that follows thetwo forward slash characters (//) on that line will not be processed by the JavaScript interpreter.

### VARIABLE
name for this concept because the data stored in a variable can change (or vary) each time a script runs. 

#### declare variable 
<img src = 'https://image.slidesharecdn.com/javascript-121025014225-phpapp01/95/javascript-by-geetanjali-23-638.jpg?cb=1353989343'>

### data type
<img src = 'https://allma.si/blog/wp-content/uploads/2020/10/data-type-in-javascript.png'>

### RULES FOR NAMING VARIABLES
1- begin with letter,$,_

2- not use -, (,)

3- You cannot use keywords or reserved words

4- All variables are case sensitive

### ARRAYS
An array is a special type of variable. It doesn't just store one value; it stores a list of values. 




# Decision & Loops
### if condition
<img src = 'https://miro.medium.com/max/1400/1*uENzVnU4d_rXpuoe9q1jsw.png'>

### comparison operator
name of operator        | description   
------------------------|----------------------
Equal (==)              | Returns true if x==y in value
Not equal (!=)          | Returns true if X !=y value
Greater than (>)        | Returns true if x>y 
Greater or equal (>=)   | Returns true if x>y or x==y
strict equal(===)       | return true in same data

### logical operator
name of operator        | description   
------------------------|----------------------
AND (&&)                | T and T =T anything else false
OR (\\\\)                   | F or F = F anything else true
not (!)                 | !true = false !false = true


### switch statement 
<img src = 'https://www.bookofnetwork.com/images/javascript-images/JS_switch-syntax_20Sep16_1827.png'>

### for statement
A for loop repeats until a specified condition evaluates to false.
loops through a block of code a number of times.

#### for (statement 1; statement 2; statement 3) {
#### // code block to be executed }

Statement 1 is executed (one time) before the execution of the code block.

Statement 2 defines the condition for executing the code block.

Statement 3 is executed (every time) after the code block has been executed.


### while statement
olops through a block of code as long as a specified condition is true.

#### while (condition) {
#### // code block to be executed }