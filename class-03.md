#### HTML CH3: LISTS 
`<ol>` - ordered list 
`<li>` - list item 
you can nest lists 

#### HTML CH13: BOXES 
Box dimensions: by default boxes are sized to be big enough to hold its contents.  But you can adjust this using width and height propertiesin CSS with values: pixels, percentages, ems.

When using % values, the % is relative to the size of the browser window or containing element.  
*Ex*: if a containing div width is 300px and the child element width is 75%, that means 75% of 300 (which is 225)

ems: the size of the box is based on the size of text within that box

Max/min-width & max/min-height -- helps ensure pages are legible when the browser window is narrowed or stretched wide 

`Overflow:` - tells browser what to do if content contained within a box is larger than the box itself.
values: hidden (hides content) & scroll (add scrollbar)

Every box has: *border, margin, padding* 

Shorthand for border property -- border: widthvalue stylevalue colorvalue l
Shorthand for margin/pading -- values: topvalue rightvalue bottomvalue left value (clockwise from top)

Padding and margin are not inherited by child so must specifify those properties on each box 

**Centering Content**: 
- set left and rgith margin to auto 
- to center box you also need to set a width 
- text-align (property) also needs to be in the mex and set value to center 
- text-align IS inhertied by children so if you don't want content to be center you need to specify in the preceding child elements 

Display (property) & values: 
- inline (makes block element act like inline element)
- block (makes inline element act like a block element)
- inline-block (block flows inline but keeps some block features)
- non (hides element from pages)

*Explanation of li's and navigation on pg. 317* 

Visibility (property): allows you to to hide boxes but leaves space where it should have been displayed (this is dissimilar to display:none).  Values: hidden, visible 

Border-image (property): applies image to border of any box (takes backgroudn image and slices in 9 peieces), requires 3 pieces of info: 
1. url
1. where to slice image 
1. what to do with straight edges 

Box-shadow (property)
Border-radius (property) - will get you roubd corners, or different shapes like circles depending on values 

#### JS CH4: P162-182 DECISIONS AND LOOPS CONT. 
*Type coercion*: when JS converts data types behind the scenes to avoid an error.  That is why it is important to use strictly 

*Truthy Values* treated as if 1.  This constitutes: 
- traditional boolean of true 
- numbers other than 0
- strings with content 
- number calculations 
- true written as a string 
- false written as a string 

*Falsy Values* treated as if 0.  This constitutes: 
- boolean false
- the number 0 
- an emptry string 
- NaN 
- variable with no assigned value (ex: var potatoe;)

*LOOPS*: checks a condition and if true runs code.  There are three types of loops: 
1. for loop (use when number of times want to code to run is known)
1. while (when when the number of times is unknown)
1. do while (will always run even if condition is false DO THIS... while)

Good visual of loops of pg. 172 

For loops are made of us 3 statements: 
1. initialization 
1. condition 
1. update 