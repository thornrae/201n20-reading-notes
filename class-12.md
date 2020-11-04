# Reading Class 12: Chart.js, Canvas

### EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS
https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/

Chart.js is a javascript plugin that uses HTML5's canvas element to draw the graph onto the page.  It makes using pies, charts, graphs really easy. 

Create data in the same script tag that is included at the foot of your HTML page. 

Always use an id attribute on your canvas element so that you can retrieve the element in the script tag to create the graph

Then you add the chart's data which is more less labels and datasets with data but line graph v pie graph etc all have different syntax


https://www.chartjs.org/docs/latest/ 

### BASIC USAGE OF CANVAS
https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage
Should give canvas element width and height attributes but defaults to a size if you don't

To grab the canvas element: 

var ctx = document.getElementById('myChart).textContent('2d);

Create fallback content using an if else statement

### DRAWING SHAPES WITH CANVAS
https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes

*The Grid*: Origin of the grid is positioned in the top left corner at coordinate (0,0).  All elements are placed relative to this origin.

Canvas only supposed rectangles and paths (which are lists of points connected by lines).  All other shapes must be created by combining one or more paths. 

Functions that draw rectangles on the canvas: 
- fillRect(x, y, width, height) : draws a filled rectangle
- strokeRect(x, y, width, height) : draws a rectangular outline
- clearRect(x,y,width,height) : clears the specified area making it fully transparent
    * x & y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle and width and height provide the rectangle's size 

*Paths* A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color.  

Internally, paths are stored as a list of sub-paths (lines, arcs, etc) which together form a shape.  Every time this method is called, the list is reset and we can start drawing new shapes.

*To Create A Path* 
- beginPath() : creates new path. once created future drawing commands are directed into the path and used to build the path up
- Path methods : methods to set different paths for objects
- closePath() : adds a straight line to the path, going to the start of the current sub-path. This is an optional step. 
- stroke() : draws the shape by stroking its outline
- fill () : draws a solid shape by filling the paths content areas

*Moving the pen* using the moveTo(x,y) function
- useful function that doesn't actually draw anything but becomes part of the path list described above.  Think of it as lifting a pen from one spot on a piece of paper and placing it on the next.  Good for using when drawing to unconnected paths - like a smiley face

*Lines* lineTo(x,y) function takes in x and y which are the coordinated of the line's end point. The starting point is dependent on previously drawn paths. Starting point can be changed using the moveTo() method

*Arcs and Circles* use:
- arc(x,y, radius, startAngle, endAngle, anticlockwise) 
    - x & y = coordinates of the center of the circle on which the arc should be drawn
    - radius is radius
    - startAngle & endAngle define the start and end points of the arc in radians along the curve of the circle. These are measured from the x axis 
    - anticlockwise is a boolean value which, when true, draws the arc anticlockwise. false = clockwise 
- arcTo(x1, y1, x2, y2, radius)

*Quadratic Bezier Curves* use this to make things like speech balloons or hearts

Use two for loops to draw a grid of rectangles
### APPLYING STYLES AND COLORS
https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors

Too apply colors to a shape: 
- fillStyle = color (sets the style used when filling shapes)
- strokeStyle = color (sets the style for shapes' outlines)

*Transparency* use globalAlpha property set equal to a transparencyValue (between 0.0 and 1.0) or you could use rgba. a = transparency

You can style lines/widths a variety of ways

To make lines crisp, understand that if your starting coordinates are (3,5) with a line width of 1pt - will put the line .5 on either side of that x axis pixel point that already exists in the computer browser. To make a crisp line you would want to choose starting coordinates 2.5. So that the width of the line matches up with the pixel on the computer

*lineCap property*: butt (squared off at endpoints), round or square values (ends of lines are squared off by adding a box with equal width and half the heigh of the line's thickness)

*lineJoin property*: determines how two connected segments of lines or arcs or curves with non zero lengths in a shape are joined together.  There are three possible values for this property: 
- round = rounds of corners of shape by filling an additional sector of disc centered at the common endpoint of connected segments. Radius for these rounded is equal to half the line width.
- bevel = fills an additional triangular area between the common endpoint of connected segments
- miter = connected segments are joined by extending their outside edges to connect at a signle point, with the effect of filling an additional lozenge-shaped area. This setting is effected by the miterLimit property.

There truly are all kinds of things you can do to create shapes and add color and effects 

### DRAWING TEXT
https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text

The canvas rendering context provides two methods to render text: 
- fillText (text, x, y [, maxwidth])
    - fills given text with xy position, optional with max width 
- strokeText(text, x, y [, maxWidth])
    - strokes a given text at the give xy position. max width optional

Properties to use to adjust the way the text gets displayed on the canvas: 
- font = value 
- textAlign = start, end, left, right, center. default value is start
- textBaseline = top, hanging, middle, alphabetic, ideographic, bottom. default is alphabetic
- direction = ltr, rtl, inherit. default value is inherit







