#### Read:04 
#### JS CH#: Functions (Pg. 86-99)

*Functions* let you group a series of statements together to perform a specific task.  Can you reuse a function? YES, and you should to follow DRY principle 

Beacuse statemtents are not always executed when a page loads, functions are used to STORE the steps needed to create a task.  That way the script can ask the function to run AS and WHEN they are required. 

In order to ask a function to perform its task LATER it must be given name. 

*CALLING A FUNCTION* is when you ask the function to perform its task.  This must happen in order for the steps inside the function to execute or run. Statements don't run until the function is called. 
- looks like : functionName(); on a line following the function declaration 

*Function Declaration* create a function, give it a name, and write the statements needed to achieve the task inside curly braces.

Some functions NEED information when they are declared, this info is known as parameters, indicated in the parentheses following the function name. The words used for the parameters act like variable names. 

When you CALL function that need information, you specify the values it should use in the parentheses following the function name 
- These values are called arguments 
- For ex: 
`getArea (3,5)`
is the same thing as: 
`wall width = 3;`
`wallHeight = 5;`
`getArea(wallWidth, wallHeight)`

To *GET A VALUE FROM A FUNCTION* use the return keyword INSIDE the function's curly braces

To get *MULTIPLE VALUES FROM A FUNCTION* - can return more than one value by returning an array 
ex: 

function getSize (width, height, depth){
  var area = width * height
  var volume = width * height * depth
  var sizes = [area, volume]
  return sizes
}

var areaOne = getSize[3,2,3] will be position [0] in sizes array 
var volumeOne = getSize[3,2,3] will be position [1] in sizes array 

Function declaration v. Function expression; function expression looks like:
var getSize = function (width, height, depth) {
  CODE
}

Local variables are called inside a function and can only be used by that function while global variables are outside and can be used by any function. But, global variables take more computer memory because they are always needing to be there while local variables are stored or used when the function is running.

#### HTML CH4: LINKS
`<a>` is the element used to link, needed, is the href attribute.  Text between the open tag and closing tag is the text link. 

You can link to other sites or to other pages on the same site. Linking to other sites requires the absolute URL while linking to other pages of the same site only needs the file link

`'target: _blank` is an attribute used with the a element that will open the page in a new window. 

You can also link to a specific part of a page by including /#idAttributeName to the end of the href link used

#### HTML CH15: LAYOUTS 
CSS treats elements as inline or block.  

If one block elements sits inside another block-level box then the ohter box is known as the containing or parent element 

*CONTROL THE POSITION OF BOXES THRU THE POSITION PROPERTY*
- position: static -- normal flow, elements on top of each other 
- position: relative +offset box properties -- indicate how far to move the element from where it would have been in normal flow 
- posotion: absolute +offset box properties -- moves box out of normal flow and no longer affects position of other elements on the page
- position: fixed +offset box properties -- positions the element in relation to the browser window.  When a user scrolls it stays in the exact same position 

*Z-INDEX PROPERTY* the higher the number the closer that element is to the top

*FLOATING PROPERTY* values: left or right 
- takes an element in normal flow and places it as far to the left or right of the containing element as possible.  Good to use the width property with this as well. 
- You can use this element to place elements side by side 

You can create multi column layouts with float, width and margin properties 

A good catch all for width of page that designers use is a width between 960-1000 

*FIXED WIDTH LAYOUTS* 
- doesn't change with the users browser window adjustments 
- specified in pixels 
- pg. 383


*LIQUID LAYOUTS* 
- stretches and contracts with the users browser window adjustments 
- specified in percentages 
- pg. 385 

*LAYOUT GRIDS* 
- 960 pixel grid - widely used by designers, (possible layout examples on pg. 390)
- also can get template from online and update with own html attributes id and class to tailor the template to your page 