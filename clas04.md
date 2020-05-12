# Read: 04 - HTML Links, CSS Layout, JS Functions

## Links:
* HTML links are hyperlinks.
* You can click on a link and jump to another document.
* When you move the mouse over a link, the mouse arrow will turn into a little hand.
> Note: A link does not have to be text. It can be an image or any other HTML element.

`HTML Links - Syntax`
`Hyperlinks are defined with the HTML <a> tag:`
`<a href="url">link text</a>`
* The href attribute specifies the destination address of the link.
* The link text is the visible part (Visit our HTML tutorial).
* Clicking on the link text will send you to the specified address.
## Local Links
The example above used an absolute URL (a full web address).
A local link (link to the same web site) is specified with a relative URL (without https://www....).
`Example`
`<a href="html_images.asp">HTML Images</a>`

## HTML Links - The target Attribute
The target attribute specifies where to open the linked document.
The target attribute can have one of the following values:
`_blank - Opens the linked document in a new window or tab`
`_self - Opens the linked document in the same window/tab as it was clicked (this is default)`
`_parent - Opens the linked document in the parent frame`
`_top - Opens the linked document in the full body of the window`
`framename - Opens the linked document in a named frame`
`This example will open the linked document in a new browser window/tab:`
`Example`
`<a href="https://www.google.com/" target="_blank">Visit W3Schools!</a>`
> Tip: If your webpage is locked in a frame, you can use target="_top" to break out of the frame:
`Example`
`<a href="https://www.google.com/" target="_top">HTML tutorial!</a>`

**HTML Links - Image as a Link**
It is common to use images as links:
`Example`
`<a href="default.asp">`
  `<img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;border:0;"></a>`
**Button as a Link**
To use an HTML button as a link, you have to add some JavaScript code.
JavaScript allows you to specify what happens at certain events, such as a click of a button:
`Example`
`<button onclick="document.location = 'default.asp'">HTML Tutorial</button>`
**Link Titles**
The title attribute specifies extra information about an element. The information is most often shown as a tooltip text when the mouse moves over the element.
`Example`
`<a href="https://www.google.com/html/" title="Go search section">Visit our HTML Tutorial</a>`

Elements/Attribute  |  Description
---------|---------
  `<a>`    |  The overflow is not clipped. It renders outside the element's box. This is default	
 `href`    |  Specifies bold text without any extra importance.
 `target`  |  The overflow is clipped, but a scroll-bar is added to see the rest of the content	
 `<img>`   |  If overflow is clipped, a scroll-bar should be added to see the rest of the content	

## Layout
> Building Blocks CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box. Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors.
**Block-level elements**
start on a new line
Examples include:
`<h1> <p> <ul> <li>`

**Inline elements**
flow in between surrounding text
Examples include:
`<img> <b> <i>`

**Containing Elements**
> If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element. It is common to group a number of elements together inside a `<div>` (or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The `<div>` element that contains this group of elements is then referred to as the containing element.

**Controlling thePosition of Elements**
> The position property specifies the type of positioning method used for an element.
Elements are then positioned using the top, bottom, left, and right properties. However, these properties will not work unless the position property is set first. They also work differently depending on the position value.
**position: static;**
HTML elements are positioned static by default.
Static positioned elements are not affected by the top, bottom, left, and right properties.
An element with position: static; is not positioned in any special way; it is always positioned according to the normal flow of the page:
This `<div>` element has position: static;
Here is the CSS that is used:
`Example`
`div.static {`
  `position: static;`
  `border: 3px solid #73AD21;}`

**position: relative**
An element with position: relative; is positioned relative to its normal position.
Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.
This `<div>` element has position: relative;
Here is the CSS that is used:
`Example`
`div.relative {`
  `position: relative;`
  `left: 30px;`
  `border: 3px solid #73AD21;}`

**position: fixed**
An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element.
A fixed element does not leave a gap in the page where it would normally have been located.
Notice the fixed element in the lower-right corner of the page. Here is the CSS that is used:
`Example`
`div.fixed {`
  `position: fixed;`
  `bottom: 0;`
  `right: 0;`
  `width: 300px;`
  `border: 3px solid #73AD21;}`

**position: absolute**
An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).
However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.
> Note: A "positioned" element is one whose position is anything except static.
`Example`
`div.relative {`
  `position: relative;`
  `width: 400px;`
  `height: 200px;`
  `border: 3px solid #73AD21;}`
`div.absolute {`
  `position: absolute;`
  `top: 80px;`
  `right: 0;`
  `width: 200px;`
  `height: 100px;`
  `border: 3px solid #73AD21;}`

**position: sticky**
An element with position: sticky; is positioned based on the user's scroll position.
A sticky element toggles between relative and fixed, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place(like position:fixed).
`Example`
`div.sticky {`
  `position: -webkit-sticky; /* Safari */`
  `position: sticky;`
  `top: 0;`
  `background-color: green;`
  `border: 2px solid #4CAF50;}`

**Overlapping Elements**
When elements are positioned, they can overlap other elements.
The z-index property specifies the stack order of an element (which element should be placed in front of, or behind, the others).
An element can have a positive or negative stack order:
`Example`
`img {`
  `position: absolute;`
  `left: 0px;`
  `top: 0px;`
  `z-index: -1;}`

![Overlapping Elements](https://i.ytimg.com/vi/09wolz1jaqE/maxresdefault.jpg)

## JS Functions, Methods, and Objects

**Functions**
A JavaScript function is a block of code designed to perform a particular task.
A JavaScript function is executed when "something" invokes it (calls it).
`Example`
`function myFunction(p1, p2) {`
  `return p1 * p2;   // The function returns the product of p1 and p2}`
> JavaScript Function Syntax
A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().
Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).
The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)
`The code to be executed, by the function, is placed inside curly brackets: {}`
`function name(parameter1, parameter2, parameter3) {`
 ` // code to be executed}`
* Function parameters are listed inside the parentheses () in the function definition.
* Function arguments are the values received by the function when it is invoked.
* Inside the function, the arguments (the parameters) behave as local variables.

**Function Invocation**
* The code inside the function will execute when "something" invokes (calls) the function:
* When an event occurs (when a user clicks a button)
* When it is invoked (called) from JavaScript code
* Automatically (self invoked)

**Function Return**
* When JavaScript reaches a return statement, the function will stop executing.
* If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.
* Functions often compute a return value. The return value is "returned" back to the "caller":
`Example`
`Calculate the product of two numbers, and return the result:`
`var x = myFunction(4, 3);   // Function is called, return value will end up in x`
`function myFunction(a, b) {`
  `return a * b;             // Function returns the product of a and b }`
`The result in x will be:  12`

**Why Functions?**
* You can reuse code: Define the code once, and use it many times.
* You can use the same code many times with different arguments, to produce different results.

## pair programming
> pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

### Why using pair program?
* 1. Greater efficiency
* 2. Engaged collaboration
* 3. Learning from fellow students
* 4. Social skills
* 5. Job interview readiness
* 6. Work environment readiness
























