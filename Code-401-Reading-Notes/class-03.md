# class-03

## What Is a File?
a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable.

#### Files on most modern file systems are composed of three main parts:
* Header: metadata about the contents of the file
* Data: contents of the file as written by the creator or editor
* End of file (EOF): special character that indicates the end of the file

### File Paths
The file path is a string that represents the location of a file. It’s broken up into three major parts:
* Folder Path: the file folder location on the file system 
* File Name: the actual name of the file
* Extension: the end of the file path pre-pended with a period

### Line Endings
The line ending has its roots from back in the Morse Code

### Character Encodings
An encoding is a translation from byte data to human readable characters. This is typically done by assigning a numerical value to represent a character.

### Opening and Closing a File in Python
<img src='https://pynative.com/wp-content/uploads/2021/06/python-file-open.png'/>
<img src='https://images.slideplayer.com/64/11811821/slides/slide_6.jpg'/>

#### Buffered Binary File Types
A buffered binary file type is used for reading and writing binary files. 

#### Raw File Types
A raw file type is:
“generally used as a low-level building-block for binary and text streams.”
 #### rideline
 <img src='https://www.edureka.co/blog/wp-content/uploads/2020/02/readlines.png'/>
 
 #### Write in file 
 * .write(string) :	This writes the string to the file.
 * 
Method	What It Does
.write(string) : This writes the string to the file.
.writelines(seq) : This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you to add the appropriate line ending(s).
 
 ## Python Exceptions: An Introduction
 ### Exceptions versus Syntax Errors
 ** Syntax errors ** occur when the parser detects an incorrect statemen
 ### Raising an Exception
 We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.
<img src='https://tutorial.eyehunts.com//wp-content/uploads/2018/10/Python-raise-exception-with-custom-message-Manually-raising.png'/> 
 ### The AssertionError Exception
 We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue
 
 ### The try and except Block: Handling Exceptions
 The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.
 <img src='https://image.slidesharecdn.com/djangoprecompiler-130113213208-phpapp02/95/web-development-with-python-and-django-31-638.jpg?cb=1358152767'/>
 
