# Read-06

### JS CH.3: OBJECT LITERALS
*Objects* group together a set of variables and functions

In objects: 
variables ---> properties 
functions ---> methods 

The value of properties can be: string, number, boolean, array, another object 

The value of a method is always a function 

**Syntax and Structure**

Declare as a variable, curly brackets, properties listed as key value pairs, properties separated by commas (except for last one), closing curly ends with a semi-colon

Access properties and methods using dot notation, assign it to a variable so you can use it later for ex: 
`var hotelName = hotel.Name;`

### JS CH.5: DOM
- The DOM is neither JavaScript nor HTML. It has its own separate set of rules 
- When a browser loads a web page it makes a model of the page in its memory
- It is called an object model because it is made up of objects
- The DOM is often referred to as an API.  API's let humans interact with programs and sets limits and rules as to how they are able to interact with them

**DOM TREE** is a model of a webpage.  It i s made up of nodes = every element, attribute and piece of text. 
- Top of tree is called document node
- Scripts access and update the DOm tree (not the HTML source file) - changes are then reflected in the browser 

**ACCESSING THE DOM** is done using queries which will return a single node value or a nodeList

*DOM QUERIES THAT RETURNS SINGLE ELEMENT*
- `getElementById('idName');` element must have attribute to be selected 
- querySelector('CSS Selector Syntax'); method returns only the first of the matching elements 

*DOM QUERIES THAT RETURNS MULTIPLE ELEMENTS*
- getElementsByClass('class-Name'); 
- getElementsByTagName('tag-name');
- querySelectorAll('CSS selector syntax'); (not supported in older browsers)

A *Nodelist* is a collection of element nodes.  Each node is given an index (which starts at 0 like an array) but they aren't actually an array.  Literally is called a collection. 

*Nodelist properties* 
- .length
- item() - returns specific node from nodelist, required parameter is the collection index you are wanting to access 

*Selecting an element from a Nodelist* using the item() method. First, smart to check if there is a tleast one node in nodelist and then use an if statement. For ex: 

var elements = document.getElementsByClassName('hot');
if (elements >= 1) {
  var firstItem = elements[0];
}

var firstItem = elements[0]; is the same thing as var firstItem = elements.item(0) but line 52 is better

You can loop thru nodlists to make changes to multiple nodes

Built in methods = 
- nodeValue - should text content of node 
- replace(old, new) - to update nodeValue text content 
- textContent - update text w/ text 
- innerText (should be avoided)

Accessing and Updating Text and Markup with Inner HTML
1. store the first list item in a variable 
1. Get the contet of the first list item
1. update ontent of the first list item so that it has new or updated content

But, you can do this PLUS create and add elements using DOM manipulation by: 
1. create element - createElement()
1. give it content - createTextNode()
1. append to DOM - appendChild()

You can also REMOVE elements 
1. select and store the element to remove 
1. select and store its containing element 
1. remove the element ( containerEl.removeChild(removeEl))

Check for an attribute and get its values using the hasAttribute() method.  Use with an if statement ex: 
1. if has has attribute
1. get that attribute
1. add value to that attribute 
`if(firstItem.hasAttribute('class')){  
  var attr = girstItem.getAttribute('class');
}

Change/create attributes and their values using className()
1. Get the first item
1. changes its class attribute (firstItem.className = 'complete')
1. get 4th item 
1. add an attribute to it (fourthItem.setAttribute('class', 'cool'))

Remove Attributes 
1. get the first item
1. if it has a class attribute (if(firstItem.hasAttribute('class')))
3. remove its class attribute (firstItem.removeAttribute('class'))



