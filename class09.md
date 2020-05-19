# Forms
The HTML `<form>` element defines a form that is used to collect user input:
An HTML form contains form elements.
Form elements are different types of input elements, like: text fields, checkboxes, radio buttons, submit buttons, and more.

Text Fields
* `<input type="text">` defines a single-line input field for text input.
* `Example`
* `A form with two text input fields:`
* `<form>`
*  `<label for="fname">First name:</label><br>`
*  `<input type="text" id="fname" name="fname"><br>`
*  `<label for="lname">Last name:</label><br>`
* ` <input type="text" id="lname" name="lname">`
* `</form>`

Attribute    |  Description
---------|---------
accept-charset  |  Specifies the charset used in the submitted form (default: the page charset).	
action  |  Specifies an address (url) where to submit the form (default: the submitting page).
autocomplete   |  Specifies if the browser should autocomplete the form (default: on).
method    |  Specifies the HTTP method used when submitting the form (default: GET).
name  |  Specifies a name used to identify the form (for DOM usage: document.forms.name).
target  |  Specifies the target of the address in the action attribute (default: _self).


## Tables

> Defining an HTML Table
An HTML table is defined with the <table> tag.
Each table row is defined with the <tr> tag. A table header is defined with the <th> tag. By default, table headings are bold and centered. A table data/cell is defined with the <td> tag.

* `Example`
* `<table style="width:100%">`
*  `<tr>`
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

**Summary**
* In addition to the CSS p XX roperties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.
* List markers can be given different appearances
using the list-style-type and list-style image
properties.
* Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.
* Forms are easier to use if the form controls are
vertically aligned using CSS.
* Forms benefit from styles that make them feel more
interactive.

## Events
* Events are the browser's way of indicating when
something has happened (such as when a page has
finished loading or a button has been clicked).
* Binding is the process of stating which event you are
waiting to happen, and which element you are waiting
for that event to happen upon.
* When an event occurs on an element, it can trigger a
JavaScript function. When this function then changes
the web page in some way, it feels interactive because
it has responded to the user.
* You can use event delegation to monitor for events
that happen on all of the children of an element.
* The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events.