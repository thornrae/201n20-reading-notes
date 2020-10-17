# READ07: HTML Tables; JS Constructor Functions
HTML CH.6: TABLES (126-125)
JS CH.3: FUNCTIONS, METHODS & OBJECTS (106-144)

### HTML CH.6: TABLES (126-125) 
Use the `<table>` element to add tables to a web page 

Tables are drawn out ROW by ROW, which are created using  `<tr>`

The cells in each row and represented by the `<td>` element BUT use `<th>` for header data

If you want to make cells of  table span more than one row or column you can use the `<rowpan></rowpan>` and `<colspan></colspan>` elements

For long tables it can be helpful to split the table into a `<thead>` `<tbody>` and `<tfoot>`

### JS CH.3: FUNCTIONS, METHODS & OBJECTS (106-144)

Constructor's are like factories that pump out objects.  So, rather that creating a bunch of objects for different types of data (for example multiple store locations with the same properties) you can create a CONSTRUCTOR. 

Constructor Syntax: 
- declare a function
- name the function - name will always start with a capital letter this is how we identify that it is a constructor 
- list the properties that are going to be with in the constructor as parameters in the parentheses and follow with curly brackets
- inside the curly braces properties look like:  this.parametername = parametername;
- methods look like: this.methodname = function () { stuff }
- to create a new instance of an object: var objectName = new Constructor(property value, property value); 
