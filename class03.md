# Read: 03 - HTML Lists, CSS Boxes, JS Control Flow

## Lists:
### Unordered HTML List
> An unordered list starts with the `<ul>` tag. Each list item starts with the `<li>` tag.
The list items will be marked with bullets (small black circles) by default:
* Example
* `<ul>`
*  `<li>Coffee</li>`
*  `<li>Tea</li>`
*  `<li>Milk</li>`
* `</ul>`

### ordered HTML List
> An ordered list starts with the `<ol>` tag. Each list item starts with the `<li>` tag.
The list items will be marked with numbers by default:
* Example
* `<ol>`
*  `<li>Home</li>`
*  `<li>Contact</li>`
*  `<li>Location</li>`
* `</ol>`

### HTML Description Lists
> HTML also supports description lists.
A description list is a list of terms, with a description of each term.
The `<dl>` tag defines the description list, the `<dt>` tag defines the term (name), and the `<dd>` tag describes each term:
* Example
* `<dl>`
*  `<dt>Coffee</dt>`
*  `<dd>- black hot drink</dd>`
* `<dt>Milk</dt>`
*  `<dd>- white cold drink</dd>`
* `</dl>`

## Boxes:
### Boxes dimenstions:
> The width and height you assign to an element is applied only to the element's content box. 
`div.box {`
`height: 300px;`
`width: 300px;` 

### Limiting Width:
> The `max-width` CSS property sets the maximum width of an element. It prevents the used value of the width property from becoming larger than the value specified by `max-width.`

> `min-width` The min-width property defines the minimum width of an element.
If the content is smaller than the minimum width, the minimum width will be applied.

### overflow:
The overflow property specifies what should happen if content overflows an element's box.
This property specifies whether to clip content or to add scrollbars when an element's content is too big to fit in a specified area.
> Note: The overflow property only works for block elements with a specified height.

Value    |  Description
---------|---------
visible  |  The overflow is not clipped. It renders outside the element's box. This is default	
hidden   |  Specifies bold text without any extra importance.
scroll   |  The overflow is clipped, but a scroll-bar is added to see the rest of the content	
auto     |  If overflow is clipped, a scroll-bar should be added to see the rest of the content	
initial  |  Sets this property to its default value.
inherit  |  Inherits this property from its parent element.

**Border**
The CSS border properties allow you to specify the style, width, and color of an element's border.
The border-style property specifies what kind of border to display.
* The following values are allowed:
* dotted - Defines a dotted border
* dashed - Defines a dashed border
* solid - Defines a solid border
* double - Defines a double border
* groove - Defines a 3D grooved border. The effect depends on the border-color value
* ridge - Defines a 3D ridged border. The effect depends on the border-color value
* inset - Defines a 3D inset border. The effect depends on the border-color value
* outset - Defines a 3D outset border. The effect depends on the border-color value
* none - Defines no border
* hidden - Defines a hidden border
> The border-style property can have from one to four values (for the top border, right border, bottom border, and the left border).

**Margin**
The margin property sets the margins for an element, and is a shorthand property for the following properties:
* margin-top
* margin-right
* margin-bottom
* margin-left

If the margin property has four values:
* margin: 10px 5px 15px 20px;
* top margin is 10px
* right margin is 5px
* bottom margin is 15px
* left margin is 20px

**Padding**
The padding property is a shorthand property for:
* padding-top
* padding-right
* padding-bottom
* padding-left
 > Note: Padding creates extra space within an element, while margin creates extra space around an element.

If the padding property has four values:
* padding:10px 5px 15px 20px;
* top padding is 10px
* right padding is 5px
* bottom padding is 15px
* left padding is 20px

![margin, border, and padding](https://www.computerhope.com/jargon/p/padding.jpg)

**Border Images**
The `border-image` property allows you to specify an image to be used as the border around an element.
* The border-image property is a shorthand property for:
* border-image-source
* border-image-slice
* border-image-width
* border-image-outset
* border-image-repeat

**Box-shadow**
The `box-shadow` property attaches one or more shadows to an element.

**Rounded Corners**
The CSS border-radius property defines the radius of an element's corners. This property allows you to add rounded corners to elements.

## JS Decisions and Loops
### Switch statement:
A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

`Syntax`
`switch(expression) {`
  `case x:`
    `// code block`
    `break;`
  `case y:`
    `// code block`
    `break;`
  `default:`
    `// code block`
`}`

* This is how it works:
* The switch expression is evaluated once.
* The value of the expression is compared with the values of each case.
* If there is a match, the associated block of code is executed.
* If there is no match, the default code block is executed.

**Switching Details**
* If multiple cases matches a case value, the first case is selected.
* If no matching cases are found, the program continues to the default label.
* If no default label is found, the program continues to the statement(s) after the switch.

**Strict Comparison**
* Switch cases use strict comparison (===).
* The values must be of the same type to match.
* A strict comparison can only be true if the operands are of the same type.
* In this example there will be no match for x:

### Loops:
Loops are handy, if you want to run the same code over and over again, each time with a different value.

**For loop**
`The for loop has the following syntax:`
`for (statement 1; statement 2; statement 3) {`
 ` // code block to be executed`
`}`
* Statement 1 is executed (one time) before the execution of the code block.
* Statement 2 defines the condition for executing the code block.
* Statement 3 is executed (every time) after the code block has been executed.
`Example`
`for (i = 0; i < 5; i++) {`
 ` text += "The number is " + i + "<br>";`
`}`
* From the example above, you can read:
* Statement 1 sets a variable before the loop starts (var i = 0).
* Statement 2 defines the condition for the loop to run (i must be less than 5).
* Statement 3 increases a value (i++) each time the code block in the loop has been executed.

**While loop**
The while loop loops through a block of code as long as a specified condition is true.
`Syntax`
`while (condition) {`
  `// code block to be executed`
`}`
* Example
`In the following example, the code in the loop will run, over and over again, as long as a variable (i) is less than 10:`
`while (i < 10) {`
  `text += "The number is " + i;`
  `i++;`
`}`




**do/while loop**
The do/while loop is a variant of the while loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.
`Syntax`
`do {`
 ` // code block to be executed`
`}`
`while (condition);`
* Example
The example below uses a do/while loop. The loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested:
`do {`
  `text += "The number is " + i;`
  `i++;`
`}`
`while (i < 10);`

> Do not forget to increase the variable used in the condition, otherwise the loop will never end!











