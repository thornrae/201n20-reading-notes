# Read 14a: CSS TRANSOFRMATIONS, TRANSITIONS AND ANIMATIONS

### TRANSFORMS
https://learn.shayhowe.com/advanced-html-css/css-transforms/

The TRANSFORM property: comes in 2D or 3D settings

Moves objects along axes (depeding on 2D or 3D / desired effect)

2D TRANSFORM:
- works on the x and y axes
- values: 
    - rotate(20deg); can rotate positive or negative degrees
    - scale(number) - default scale value is 1 so any value between .99 and .01 makes element appear smaller and anything grater than or equal to 1.01 makes an element appear larger  
    - skew(20deg), skewX or skewY

3D TRANSFORM: 
- works on x y and z axes

You can combine different transforms to create perspective changes or 3D figures

### TRANSITIONS
https://learn.shayhowe.com/advanced-html-css/transitions-animations/

Have the ability to alter the apperance and behavior of an element whenver a state change occurs (such as hovered over, focused on, activated or targeted)

In order to take place the element must have a change in state and different styles must be identitified for each state (:hover, :focus, :active, :target)

Four transition related properties:
1. transition-property
1. transition-duration 
1. transition-timing-function 
1. transition-delay
    * not all are required to build a transition but first three are most popular

Not all properties may be transitioned here are some popular ones: 
background-color background-position border-color border-width border-spacing bottom clip color crop font-size font-weight height left letter-spacing line-height margin max-height max-widt hmin-height min-width opacity outline-color outline-offset outline-width padding right text-indent text-shadow top vertical-align visibility
width word-spacing z-index

*Duration* can be listed as s or ms can can .2 - do not need to be whole number

**Look at this article link for: card flip, bouncing ball**

### 8 SIMPLE CSS TRICKS TO WOW USERS 
http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/

This article shows: 
- fade in 
- change color
- grow
- shrink
- rotate
- squre to circle
- 3D shadow 
- swing
- inset border

Animated buttons: https://codepen.io/retyui/pen/ByoaXV 
Key frames animation: https://codepen.io/akshaychauhan/pen/oAfae 
404 Error Moving: https://codepen.io/kieranfivestars/pen/MYdQxX
Bound Animation: https://codepen.io/dp_lewis/pen/gCfBv 