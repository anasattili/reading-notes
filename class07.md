# Read: 07 - HTML Tables; JS Constructor Functions

## HTML Tables:
An HTML table is defined with the `<table>` tag.

Each table row is defined with the <tr> tag. A table header is defined with the <th> tag. By default, table headings are bold and centered. A table data/cell is defined with the <td> tag.

**Example**
* `<table style="width:100%">`
* `<tr>`
*   `<th>Firstname</th>`
*    `<th>Lastname</th>`
*    `<th>Age</th>`
*  `</tr>`
*  `<tr>`
*    `<td>Jill</td>`
*    `<td>Smith</td>`
*    `<td>50</td>`
*  `</tr>`
*  `<tr>`
*    `<td>Eve</td>`
*    `<td>Jackson</td>`
*    `<td>94</td>`
*  `</tr>`
* `</table>`

> Note: The <td> elements are the data containers of the table.
They can contain all sorts of HTML elements; text, images, lists, other tables, etc.

## Functions, Methods, and Objects in JavaScript

A JavaScript function is a block of code designed to perform a particular task.
A JavaScript function is executed when "something" invokes it (calls it).
`Example`
`function myFunction(p1, p2) {`
 ` return p1 * p2;   // The function returns the product of p1 and p2}`

**creat object constructor notation in javascript**
![constructor](https://hsheikhm.files.wordpress.com/2016/02/screen-shot-2016-02-13-at-21-54-14.png?w=584)

Accessing JavaScript Properties
The syntax for accessing the property of an object is:
* `objectName.property         // person.age`
* `objectName["property"]      // person["age"]`
* `objectName[expression]      // x = "age"; person[x]`

**ADDING AND REMOVING PROPERTIES** 
* `var hotel = {`
* `name : 'Park' ,`
* `rooms : 120,`
* `booked : 77.`
* `} ;`
* `hotel .gym = t rue;`
* `hotel .pool = fal se;`
* `delete hotel .booked;`
* `var elName = document .getEl ementByld('hotelName ' );`
* `elName.textContent = hotel . name;`
* `var el Pool = document .getElementByid ('pool ') ;`
* `elPool.cl assName = ' Pool: ' + hotel. pool ;`
* `var elGym = document .getEl ementByld('gym ' };`
* `elGym.className = 'Gym: ' + hotel .gym;`

**THIS (IT IS A KEYWORD)**
> The keyword this is commonly used inside functions and objects.
Where the function is declared alters what this means. It always refers
to one object, usually the object in which the function operates.

![constructor](https://4.bp.blogspot.com/-4-NK6MDoeGE/XQuKB9TyulI/AAAAAAAAYaw/y8yvA1afRM0t908bEoJWtn6R16PrmxvDwCLcBGAs/s400/this-keyword.PNG
)

> Browsers come with a set of built-in objects that represent things like the
browser window and the current web page shown in that window. These
built-in objects act like a toolkit for creating interactive web pages.

* BROWSER OBJECTMODEL
* GLOBAL JAVASCRIPTOBJECTS
* DOCUMENT OBJECTMODEL

## Summary:
* Functions allow you to group a set of related statements together that represent a single task.
* Functions can take parameters (informatiorJ required to do their job) and may return a value.
* An object is a series of variables and functions that represent something from the world around you.
* In an object, variables are known as properties of the object; functions are known as methods of the object.
* Web browsers implement objects that represent both the browser window and the document loaded into the
browser window.
* JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and
methods offer functionality that help you write scripts.
* Arrays and objects can be used to create complex data sets (and both can contain the other).

