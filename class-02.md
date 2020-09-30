#### JS CH2: Basic JavaScript Instructions

*Statements* make up a script.  Scripts are a series of statements that are case sensitive and end with a semi-colon.  Each one starts on a new line. 

*Variables* ... scripts store bits of information needed to run a task in variables.  Variables essentially are used to remember information. 
- Data stored in variables can change or vary each time ascript runs. 
- Variables can be used to represent values in your scripts that are likely to change
- Programmers **DECLARE** variables (this is the verbiage used to describe use of a variable in code)
- "var" is a javascript *keyword*.  A variable with no value is described as undefined.
- Where a variable is placed can have an effect upon whether the rest of the script can use it (global v local variables)

*Datatypes*: numeric, boolean or string

One a value has been assigned to a variable you can use the variable name to reprsent the value much like algebra. 

In boolean datatypes; 0 = false, 1 = true.  But, often you don't display true or false to the user, more commonly boolean data is used to trigger a certain type of CSS or display. 

When you see "document.getElementById" you say "code selects elements using the value of their id attribute". 

You can change what information is stored in a variable later in the same script.  Once a variable has been created, you don't need to use var just the name and operator (which is the equal sign)

*Rules for naming variables* 
- can't sart with a number
- name cannot contain a dish or period 
- no keywords or reserved words 
- case senstive

*Arrays* are declared the same way a variable is and uses the keyword var.  Arrays can hold more than one data type, separated by values.

Values in an array are accessed as if they are in a numbered list, starting with 0.  Each item in an array is automatically assigned a number - these numbers are referred to as the array index. You access specific items in an array by calling the index number. 

Accessing and changing values in an array: 
1. access value of array for example: `arrayName[indexValue]`
1. use operator and assign value 
1. that index location is now updated

Expressions evaluate into a single value. Broadly speaking, there are 2 types of expressions
1. expressions that assign value to a variable 
1. expressions that use two or more values to return a single value 

Expressions rely on operators which allow programmers to do the second type of type of expression where two values return a single value 

++ adds 1 to the current number 
-- subtracts 1 from the current number 

PEMDAS applies

#### JS CH4: DECISIONS AND LOOPS 
Evaluations, decisions and loops create and control the flow of data in your scripts to handle different situations.

*Evaluations* analyze values to detemine if they match expected results 
*Decisons* use results of evaluations to decide which path script should go down 
*Loops* situation where you want to perform the same set of steps repeatedly 

**Decision Making** 
- determines which path to take, set a condition 
- if condition is true -> that s path 
- if condition is false -> thats a different path 
- comparison operators allow you to compare values and test whether a condition is met or not

**Evaluating Conditions and Conditional Statements** The two components to a decision are: 
1. an expression is evaluated, which returns a value 
1. a conditional statement says what to do in a given situation, based on if, then, else logic

While comparison operators (!=, !==, ==, ===, <=, <) usually return true or false, *logical operators* (&& || ! )allow you to compare the results of more than one comparison operator.

Logical expressions are evaluated left to right.  If the first condition can provide enough information to get the answer then there is no need to evaluate the second condition 

Short cut: false && anything will return false, true || anything will return true
!true returns false 
!false returns true 

*If Statements*: checks a condition, if it evaluates to true, any statements in subsequent code block are executed

#### HTML CH2: TEXT
Structural markup v. semantic markup 

*Structural markup example tags*: h1-h6, p, b, i, sup, sub, br/, hr/
*Semantic markup* these are used to desribe contents of your page better to screenreaders.  Examples: strong, em, blockquote, abbr, dfn, address, acronym, cite, ins, s, del 

#### HTML CH10: INTRODUCING CSS
- CSS works by associated rules with HTML elements 
- CSS rules contain 2 parts: selector and declaration 
- Declarations are made up of 2 parts, property and a value

Use external CSS with the link tag and three required attributes: href (link to file path), type= "text/css", rel="stylesheet"

There are many different types of CSS selectors. Can be found on page 238. 

If there are two styles for one element, what takes precedence? 
- Last: the latter will take precdence 
- Specificity: if one selector is more specific, that will take precendence 
- `!important` - you can add this after any property value to indicate it should be considered more important than other otherrules that apply to the same element 

*Inheritence*: font family and color will apply tomost child elements. But, this is not true for CSS properties like background color or border properties.  **You can force inhertiance** for example; padding:inherit in a child element will make it inherit the padding values of its parent element 
