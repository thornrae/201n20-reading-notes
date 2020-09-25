#### JS CH1: The ABC's of Programming

Start with the big picture and break it down into smaller steps
1. Define the goal
1. Design the script (pseudocode)
1. Code each step 

Use flow charts to work out how tasks fit together.  Generic flow charts will have shapes that indicate different types of actions for example, a generic step (ex: calculate something), an event (ex: click), input or output (ex: show somethign or ask something) or decision (ex: is there a name to get?). 

*Properties*, *events* and *methods* merge together to create working models of real world objects.

**Properties** are made of key value pairs (name: value)
**Events** are the like the ways that you interact with an object.  When an event happens, that action can be used to trigger a specific section of code. Scripts often use different events to trigger different types of functionality. 
**Methods** represent things that people do to objects. They can retrieve or update the values of an objects properties.

*The Document Object* using this, you can access and change what users see on the page and respond to how they interact with it.  The document object represents the HTMl page and contains events, methods and properties (DOM)
- When the browser creates a model of a webpage, it not only creates a document object, but it also creates a new object for each element in the page.  Together that is how we get the DOM. 
- The document object has several methods and properties which are known as *members* of that object.  You need a member operator (`.`) to access members of the object.  Parameters are pieces of information that the method requires in order to do its work. For example: 
`document.write('Good Afternoon)` -- document = object; .= member operation; write = function; Good Afternoon = parameter

JavaScript is an interpreted programming language meaning that computers translate it into something it can understand to be able to carry out the function. 
- Browser creates HTML page
- Creates a model of the page and stores in its memory 
- It shows the page on the screen using a rendering engine 

*Progressive Enhancement* is the use of HTML (content layer), CSS (presentation layer), JS (behavior layer) to create web pages

We use the `<script>` tag with a `src` attribute to link a .js file to an HTML page.  It matters where you put the script tag as its placement can affect the loading time of the page as well as effect where elements appear on the page. 

#### HTML CH1: STRUCTURE 
HTML uses elements to describe the structure of pages.  Tags act like containers, they tell you somethinga about the info that lies between their opening and closing tags. 

*Attributes* provide additional information about the contents of an element and appear in the opening tag of the element. 
- Made of key value pairs 
- Written in lower case
- Values should be written in lowercase and placed in double quotes

#### HTML CH8: EXTRA MARKUP
Start all HTML documents with `<!DOCTYPE html>`. This helps page render correctly 

To comment out code highlight and command shift OR use `<!-- comment -->`

It is important to use comments not only for yourself but for other people who will read your code 

*id Attribute* 
- Uniquely identifies that element from other elements on that page 
- Value should start with a letter or underscore, NO numbers or other characters 
- No 2 elements on the page should have the same id value
- Giving an element a unique identifier allows you to style it differently in CSS
- When using js id attributes can be used to allow the script to work with that particular element 
- This is  global attribute meaning that it can be used on any element 

*class Attribute* 
- Use to identify several elements as being different from other elements on the page
- You can assign multiple class names to the same element, separated by a space

*Block Elements* are elements that appear to start on a new line in the browser window
- `<h1>`
- `<p>`
- `<ul>`
- `<li>`

*Inline Elements* are elements that appear to continue on the same line as their neighboring elements.  For ex: 
- `<a>`
- `<b>`
- `<em>`
- `<img>`

The *`<div>`* element allows you to group a set of elements together in one block level box 
- using id and class attributes in your div can help with styling or indicate how much space the div element should occupy on the screen 

The *`<span>`* element acts like an inline equivalent of the div element.  It is used to either 
1. Contain a section of text where there is no other suitable element to differentiate it from surrounding text
1. Contain a number of inline elements 
- It is used most often to control the appearance of the content of these elements 

*`<iframe>`* - inline frame element.  Inserts a window to another page within your page, like a google map for example. Attributes associated with this element: 
- src, height, width 
- scrolling, values = "yes" or "no" 
- framborder, values = "0" (no border) or "1" (border)

*`<meta>`* - holds information about the page 
- lives in the head and so not visible to users but used by search engines 
- empty element (no closing tag)
- uses attributes to carry information, most common of which are **name** and **content** to specifiy properties of the entire page 
- Commonly used values are: 
1. Description - commonly used by search engines; 155 character max 
1. Keybword - comma separated word list that a user might search to find the page 
1. Robots - has two values noindex (used if page should not be added to a search enginges results) or nofollow (yes add page to search results but not any page it links to)
1. Author - defines author of webpage 
1. Pragma - prevents browser from caching the page 
1. Expires - can be used to indicate if/when the page should expire.  Specific date format required. 

*Escape Characters* are characters used in code that, if you want displayed on page you need to write differently, for example an ampersand. Full list on page 194. 

#### HTML CH17: HTML5 LAYOUT
With HTML divs were used for all aspects of the page with attributes to indicate the type of content.  With HTML5 those attributes now exist as their own elements. For example: 
- `<header>`, `<footer>`, `<nav>`, `<article>`, `<aside>`, `<section>`, `<hgroup>`, `<figure>`

Also, `<a>` can be placed around a block level element that contains child elements.  This allows you to turn an entire block into a link. 

#### HTML CH18: PROCESS AND DESIGN
Site map - a diagram of the page that will be used to structure the site

Wireframing - simple sketch to show the hierarchy of information and how much space it may require 

Design techniques to keep in mind: visual hierarchy, grouping, similarity 