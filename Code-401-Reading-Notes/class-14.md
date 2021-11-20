# class_14
## matplotlib
matplotlib is probably the single most used Python package for 2D-graphics. 
#### IPython 
IPython is an enhanced interactive Python shell that has lots of interesting features including named inputs and outputs,
#### pyplot
pyplot provides a convenient interface to the matplotlib object-oriented plotting library.

#### plot command 
img src='https://editor.analyticsvidhya.com/uploads/6133521.PNG'/>

#### xlim and ylim command 
<img src='https://miro.medium.com/max/894/1*cfuTFHNgveDQn0I9JvJxAA.png'/>

#### xticks and yticks command
* plt.axes(*args, emit=True, **kwargs): For setting the axes for our plot with parameter rect as [left,bottom,width,height] for  setting axes position.
* plt.axes().set_xticks() and plt.axes().set_yticks() : For setting ticks on x-axis and y-axis respectively. having data in form of a list set as parameter.
* plt.axes().set_xlabels() and plt.axes().set_ylabels() : To set labels of our ticks with parameters in form of list.
* <img src='https://user-images.githubusercontent.com/22521393/55283695-720cf980-539b-11e9-8a0e-f8bc365719ec.png'/>

#### legend command
img src = 'https://editor.analyticsvidhya.com/uploads/32332123.PNG'/>

### Figures
A figure is the windows in the GUI that has "Figure #" as title. Figures are numbered starting from 1 as opposed to the normal Python way starting from 0. This is clearly MATLAB-style
### Subplots
With subplot you can arrange plots in a regular grid. You need to specify the number of rows and columns and the number of the plot. 
### Axes
Axes are very similar to subplots but allow placement of plots at any location in the figure. So if we want to put a smaller plot inside a bigger one we do so with axes.
### Ticks
Well formatted ticks are an important part of publishing-ready figures. Matplotlib provides a totally configurable system for ticks. There are tick locators to specify where ticks should appear and tick formatters to give ticks the appearance you want.

