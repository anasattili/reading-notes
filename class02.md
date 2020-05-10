# Read: 02 - HTML Text, CSS Introduction, and Basic JavaScript Instructions

## Text in HTML:
* When creating a web page, you add tags (known as markup) to the contents of the page.
*  An HTML tag is a special word or letter surrounded by angle brackets, < and >. You use tags to create HTML elements, such as paragraphs or links.
* Structural markup: the elements that you can use to describe both headings and paragraphs
* Semantic markup: which provides extra information; such as where emphasis is placed in a sentence.

## HTML Heading:
HTML headings are defined with the `<h1>` to `<h6>` tags. `<h1>` defines the most important heading. `<h6>` defines the least important heading.
**Search engines use the headings to index the structure and content of your web pages.**

## HTML Paragraphs:
The HTML <p> element defines a paragraph.
A paragraph always starts on a new line, and browsers automatically add some white space (a margin) before and after a paragraph.

Element  |  Function
---------|---------
`<b>`    |  Specifies bold text without any extra importance.
`<i>`    |  Defines a part of text in an alternate voice or mood. The content of the <i> tag is usually displayed in italic.
`<sup>`  | Defines superscript text. Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font. Superscript text can be used for footnotes, like WWW
`<sub>`  |  Defines subscript text. Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font. Subscript text can be used for chemical formulas, like H2O.
`<br />` | Inserts a single line break.
`<hr />` | Stands for horizontal rule and is used to insert a horizontal rule or a thematic break in an HTML page to divide or separate document sections.
`<strong>`|gives text a strong emphasis which traditionally means that the text is displayed as bold by the browser.
`<em>`   | It renders as emphasized text.
`<blockquote>`  |specifies a section that is quoted from another source. Browsers usually indent `<blockquote> `elements.
`<q>`    | Defines a short quotation. Browsers normally insert quotation marks around the quotation.
`<abbr>` | Defines an abbreviation or an acronym, like "HTML", "Mr.", "Dec.", "ASAP", "ATM".
`<cite>` | Defines the title of a work (e.g. a book, a song, a movie).
`<dfn>`  | Rrepresents the defining instance of a term in HTML. The defining instance is often the first use of a term in a document.
`<address>` | defines the contact information for the author/owner of a document or an article. The contact information can be an email address, URL, physical address, phone number, social media handle.
`<ins>` | Defines a text that has been inserted into a document.
`<del>` | Defines text that has been deleted from a document.
`<s>` | specifies text that is no longer correct, accurate or relevant.
`<ins>` | defines the title of a work (e.g. a book, a song, a movie).

## Introducing CSS:
> CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.
* Selectors indicate which element the rule applies to. The same rule can apply to more than one element if  you separate the element names with commas.
* Declarations indicate how the elements referred to in the selector should be styled. Declarations are split parts (a property and a value),into two and are separated by a colon.
> CSS declarations sit inside curly brackets and each is made up of two 
parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.
* Properties indicate the aspects of the element you want to change. For example, color, font, width, height and border.
* Values specify the settings you want to use for the chosen properties. For example, if you want to specify a color property then the value is the color you want the text in these elements to be.

## Using external css
HTML:
`<!DOCTYPE html>`
`<html>`
`<head>`
`<title>Using External CSS</title>`
`<link href="css/styles.css" type="text/css"`
`rel="stylesheet" />`
`</head>`
`<body>`
`<h1>Potatoes</h1>`
`<p>`There are dozens of different potato
varieties. They are usually described as
early, second early and maincrop.`</p>`
`</body>`
`</html>`
CSS:
`body {`
`font-family: arial;`
`background-color: rgb(185,179,175);}`
`h1 {`
`color: rgb(255,255,255);}`

## Using internal css
`<!DOCTYPE html>`
`<html>`
`<head>`
`<title>Using Internal CSS</title>`
`<style type="text/css">`
`body {`
`font-family: arial;`
`background-color: rgb(185,179,175);}`
`h1 {`
`color: rgb(255,255,255);}`
`</style>`
`</head>`
`<body>`
`<h1>Potatoes</h1>`
`<p>`There are dozens of different potato
varieties. They are usually described as
early, second early and maincrop.`</p>`
`</body>`
`</html>`

## CSS Selectors
> In CSS, selectors are patterns used to select the element(s) you want to style.
* Universal Selector: Applies to all elements in the document. 
* Type selector: Matches element names.
* Class selector: Matches an element whose class attribute has a value that matches the one specified after the period (or full stop) symbol.
* Id selector: Matches an element whose id attribute has a value that matches the one specified after the pound or hash symbol.
* Child Selector: Matches an element that is a direct child of another.
* Descendant Selector: Matches an element that is a descendent of another specified element (not just a direct child of that element).
* Adjacent sibling selector: Matches an element that is the next sibling of another.
* General sibling selector: Matches an element that is a sibling of another, although it does not have to be the directly preceding element.

## Cascading Order
All the styles in a page will "cascade" into a new "virtual" style sheet by the following rules:
* Inline style (inside an HTML element)
* External and internal style sheets (in the head section)
* Browser default
> So, an inline style has the highest priority, and will override external and internal styles and browser defaults.

## Inheritance
In CSS, inheritance controls what happens when no value is specified for a property on an element.
CSS properties can be categorized in two types:
* inherited properties, which by default are set to the computed value of the parent element.
* non-inherited properties, which by default are set to initial value of the property.

## The benefits of using an external style sheet are:
* everything is stored within a single file.
* once changed/updated, the changes are reflected on all other pages that reference the stylesheet.
* this makes it easier to maintain larger websites.
* pages load quicker once the main CSS file has been cached.

## Basic JavaScript Instructions

### Comments:
* Single line comments start with //.
Any text between // and the end of the line will be ignored by JavaScript (will not be executed).
* Multi-line comments start with /* and end with */.
Any text between /* and */ will be ignored by JavaScript.

### Variables:
JavaScript Variable
* Variable means anything that can vary. JavaScript includes variables which hold the data value and it can be changed anytime.
* JavaScript uses reserved keyword var to declare a variable. A variable must have a unique name. You can assign a value to a variable using equal to (=) operator when you declare it or before using it.
* Syntax:
* var `<variable-name>;`
* var `<variable-name> = <value>;`
* Example: Variable Declaration & Initialization
* var one = 1; // variable stores numeric value
* var two = 'two';  // variable stores string value
* var three;  // declared a variable without assigning a value
> In the above example, we have declared three variables using var keyword: one, two and three. We have assigned values to variables one and two at the same time when we declared it, whereas variable three is declared but does not hold any value yet, so it's value will be 'undefined'.
* Declare Variables in a Single Line
* Multiple variables can also be declared in a single line separated by comma.

### Data Types:
JavaScript variables can hold many data types: numbers, strings, objects, Booleans.
* `var length = 16;`                               // Number
* `var lastName = "Johnson";`                      // String
* `var x = {firstName:"John", lastName:"Doe"};`    // Object
Booleans can only have two values: true or false.
The Concept of Data Types
In programming, data types is an important concept.
To be able to operate on variables, it is important to know something about the type.

### Rules for naming variables:
* Names can contain letters, digits, underscores, and dollar signs.
* Names must begin with a letter
* Names can also begin with $ and _ (but we will not use it in this tutorial)
* Names are case sensitive (y and Y are different variables)
* Reserved words (like JavaScript keywords) cannot be used as names

### Arrays:
* JavaScript arrays are used to store multiple values in a single variable.
`var cars = ["Saab", "Volvo", "BMW"];`
* An array is a special variable, which can hold more than one value at a time. If you have a list of items (a list of car names, for example).
* Access the Elements of an Array
You access an array element by referring to the index number.
This statement accesses the value of the first element in cars:
* Example
`var cars = ["Saab", "Volvo", "BMW"];`
`var name = cars[0]; // name=Saab;`





### Operators:
* `+	Addition`
* `-	Subtraction`
* `*	Multiplication`
* `**	Exponentiation`
* `/	Division`
* `%	Modulus (Division Remainder)`
* `++	Increment`
* `--	Decrement`
* `x = y	x = y`
* `+=	x += y	x = x + y`
* `-=	x -= y	x = x - y`
* `*=	x *= y	x = x * y`
* `/=	x /= y	x = x / y`
* `%=	x %= y	x = x % y`
* `**=	x **= y	x = x ** y`
* JavaScript String Operators
The + operator can also be used to add (concatenate) strings.
Example
* `var txt1 = "John";`
* `var txt2 = "Doe";`
* `var txt3 = txt1 + " " + txt2;`

### Decisions and Loops

## Comparison condition:
* Given that `x = 5`
* `==	equal to	x == 8	false`	
* `x == 5	true`	
* `x == "5"	true`	
* `===	equal value and equal type	x === 5	true`	
* `x === "5"	false`	
* `!=	not equal	x != 8	true`	
* `!==	not equal value or not equal type	x !== 5	false`
* `x !== "5"	true`	
* `x !== 8	true`	
* `>	greater than	x > 8	false`	
* `<	less than	x < 8	true`	
* `>=	greater than or equal to	x >= 8	false`	
* `<=	less than or equal to	x <= 8	true`

### Logical Operators:
* Given that `x = 6` and `y = 3`:
* `&&	and	(x < 10 && y > 1) is true`	
* `||	or	(x == 5 || y == 5) is false`	
* `!	not	!(x == y) is true`

### Conditional Statements:
Very often when you write code, you want to perform different actions for different decisions.
You can use conditional statements in your code to do this.
In JavaScript we have the following conditional statements:
* Use `if` to specify a block of code to be executed, if a specified condition is true.
* Use `else` to specify a block of code to be executed, if the same condition is false.
* Use `else if` to specify a new condition to test, if the first condition is false.
* Examples:
* `if (hour < 18) { greeting = "Good day";}`

* `if (hour < 18) { greeting = "Good day";}`
  `else { greeting = "Good evening";}`

* ` if (time < 10) { greeting = "Good morning";}`
  `else if (time < 20) { greeting = "Good day";}`
  `else { greeting = "Good evening";}`

  

  
  
































