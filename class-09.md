# Forms and JS Events

### HTML CH7: FORMS

HTML forms gives you a set of elelemtns to collect data from your users.

Form controls: several types of these which all you to collect info from visitors:
- add text: text-input(single line), password input (single line, mmasks characters), text area(multi line) - for longer messages and comments
- make choices: radio buttons, check boxes, drop down boxes
- submitting forms: submit buttons, merge buttons file upload

Flow of forms: after submitting form, the name of each form control is sent to the server along with the value that the user enters.  Server processes the info using PHP, C#, VB.net, or Java (info could also be stored in a database). Server creates new page to send back to browser based on infomration received.

FORM STRUCTURE
`<form>` has two attributes: action (url), method
`<input>` (self closing) attributes: 
  - type = text, password; name, size, maxlength
  - type = radio w/ attributes: name, value
  - type = checkbox w/ attributes: name, value, checked
  - type = submit w/ attributes name, value. Value controls text on button. if using image for submit button use input w/ attribute type = image with src, width and height attributes
`<textarea>` - use for comments.  attributes: name, cols, rows
`<select>` `<option>` - option w attributes: value 

When using a button element you can use a hidden feature attribute 

`<label>` giving context to field forms. 

To group elements on the form: `<fieldset>` following by `<legend>` tags 

From validation attribute: required = required

### HTML CH 14: LISTS, TABLES, FORMS 
To specify type of bullet in UL: 
list-style-type: non, disc, circle, square

To specify type of bullet in OL:
list-stype-type: decimal, decimal-leading-zero, lower-alpha, upper-alpha, lower-roman, upper-roman

list-style-image: url (link to use as image for bullet point)

list-style-position: outside, inside 

Properties to use to style tables: width, padding, text-transform, letter-spacing, font-size, border-top, border-bottom, text-align, background-color,  :hover 

The emtpy-cell property: show, hide, inherit 

To style forms use properties: font-size, color, background-color, border, border-radius, background-image 

To style submit buttons: color, text-shadow, background-color

Psuedo elements: :focus & :hover

Styling fieldsets & legends: color, background-color, border, border-radius, padding

### JS CH6: EVENTS
There are 6 types of events that can occur to trigger a function in your javascript code. 
1. user interface events (UI)
1. keyboard events 
1. mouse events 
1. focus events 
1. form events 
1. mutations events aka mutation observers (when something changes in the DOM structure)

Event handling is what triggers JS code and is made up of 3 steps:

1. selecting element node 
1. indicate what event on what node will trigger response "binding to a note"
1. stat the code you want to run when the event occurs

Two ways to bind: traditional DOM event handlers and event listeners.  The latter is more dynamic because you can use it to trigger more than one function per event

Event Listener Syntax: 
element.addEventListener('event', function);

To use parameters in event listeners call the function anonymously and then call the function with parameters within the preceding curly brackets. 

THE EVENT OBJECT 
when an event occurs the event object tells you info about the event andthe element it happened upon. 

The event object is passed to any function that is the event handler or the event listener and when passed thru a function often give you the name of e (???)

Without doing anything a reference to the event object is automatically passed from step 1 to step 2 (pg. 263)

The event object also has useful build in methods