# HTML CH15: LAYOUTS
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