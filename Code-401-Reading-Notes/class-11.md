# class_11
## Jupyter Lab
JupyterLab is a next-generation web-based user interface for Project Jupyter.
<br>
You can arrange multiple documents and activities side by side in the work area using tabs and splitters. Documents and activities integrate with each other, enabling new workflows for interactive computing

<img src='https://miro.medium.com/max/955/1*mXGu0MeYgnUkyR9ybVlQpg.png'/>

* Code Consoles provide transient scratchpads for running code interactively, with full support for rich output. 
* Kernel-backed documents enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.
* Notebook cell outputs can be mirrored into their own tab, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.
* Multiple views of documents with different editors or viewers enable live editing of documents reflected in other viewers. 

## NumPy Tutorial: Data Analysis with Python

NumPy is a commonly used Python data analysis package. By using NumPy, you can speed up your workflow, and interface with other packages in the Python ecosystem, 

#### Dimensional Arrays
In a NumPy array, the number of dimensions is called the rank, and each dimension is called an axis. So the rows are the first axis, and the columns are the second axis.

#### Creating A NumPy Array
If we pass in a list of lists, it will automatically create a NumPy array with the same number of rows and columns. Because we want all of the elements in the array to be float elements for easy computation,
<img src='https://miro.medium.com/max/1250/1*frSKgQ_VFID9EDHbjbgc2A.png'/>
<br>
We can check the number of rows and columns in our data using the shape property of NumPy arrays:
<br>
You can also create an array where each element is a random number using numpy.random.rand. 
<br>
<img src='https://www.arabicprogrammer.com/images/317/94f5b83a223fb5f04428f66eee3041bd.png'/>


### Using NumPy To Read In Files
It’s possible to use NumPy to directly read csv or other files into arrays. We can do this using the numpy.genfromtxt function. We can use it to read in our initial data on red wines.

In the below code, we:

* Use the genfromtxt function to read in the winequality-red.csv file.
* Specify the keyword argument delimiter=";" so that the fields are parsed properly.
* Specify the keyword argument skip_header=1 so that the header row is skipped.

**wines = np.genfromtxt("winequality-red.csv", delimiter=";", skip_header=1)**
