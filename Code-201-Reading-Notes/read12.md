# canvas element 

The <canvas> tag is used to draw graphics, on the fly, via scripting (usually JavaScript).
<br>The <canvas> tag is transparent, and is only a container for graphics, you must use a script to actually draw the graphics.
`<canvas id="tutorial" width="150" height="150"></canvas>`
<br> When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high.
<br> The `<canvas>` element can be styled just like any normal image (margin, border, background…). These rules, however, don't affect the actual drawing on the canvas. 
<br> like for `<video>`, `<audio>`, or `<picture>`
<br> Providing fallback content is very straightforward: just insert the alternate content inside the `<canvas>` element


<img src = "https://miro.medium.com/max/1006/0*V1G6ajUNd5s2Rqy4">

### The rendering context
The `<canvas>` element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown.

<img src = "https://www.wikitechy.com/step-by-step-html-tutorials/img/html-images/code-explanation-canvas-tag-in-html.png">
  
  
  ### The grid
  Normally 1 unit in the grid corresponds to 1 pixel on the canvas.<br>
  `<canvas>` only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths.
  <br>
  
  <img src = "https://miro.medium.com/max/1400/1*RFW4A8MDdRx8LHNKryqoRQ.png">
  
  
  ### Applying styles and colors
  
  * ctx.fillStyle = 'orange';
* ctx.fillStyle = '#FFA500';
* ctx.fillStyle = 'rgb(255, 165, 0)';
* ctx.fillStyle = 'rgba(255, 165, 0, 1)';

  
  ### Drawing text
  function draw() {<br>
  var ctx = document.getElementById('canvas').getContext('2d');<br>
  ctx.font = '48px serif';<br>
  ctx.fillText('Hello world', 10, 50);<br>
}
  
  ### A strokeText
  function draw() {<br>
  var ctx = document.getElementById('canvas').getContext('2d');<br>
  ctx.font = '48px serif';<br>
  ctx.strokeText('Hello world', 10, 50);<br>
}
  ### Styling text
  * font = value
  * textAlign = value
  * textBaseline = value ,top, hanging, middle, alphabetic, ideographic, bottom
  * direction = value , ltr, rtl, inherit.
  
  ### Advanced text measurements
  function draw() {<br>
  var ctx = document.getElementById('canvas').getContext('2d');<br>
  var text = ctx.measureText('foo'); // TextMetrics object<br>
  text.width; // 16;<br>
}<br>
  
  ### A lineCap 
  The lineCap property determines how the end points of every line are drawn. There are three possible values for this property and those are: butt, round and square
  
  ### A lineJoin
  The lineJoin property determines how two connecting segments (of lines, arcs or curves) with non-zero lengths in a shape are joined together
  <br>
  There are three possible values for this property: round, bevel and miter
  
  
