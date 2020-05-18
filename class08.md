# Read: 08 - More CSS Layout

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
* HTML elements are positioned static by default.
* Static positioned elements are not affected by the top, bottom, left, and right properties.
* An element with position: static; is not positioned in any special way; it is always positioned according   to  the normal flow of the page:
* This `<div>` element has position: static;
* Here is the CSS that is used:
* `Example`
* `div.static {`
*  `position: static;`
*  `border: 3px solid #73AD21;}`

**position: relative**
An element with position: relative; is positioned relative to its normal position.
Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.
* This `<div>` element has position: relative;
* Here is the CSS that is used:
* `Example`
* `div.relative {`
*  `position: relative;`
*  `left: 30px;`
*  `border: 3px solid #73AD21;}`

**position: fixed**
An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used to position the element.
A fixed element does not leave a gap in the page where it would normally have been located.
Notice the fixed element in the lower-right corner of the page. Here is the CSS that is used:
* `Example`
* `div.fixed {`
*  `position: fixed;`
*  `bottom: 0;`
*  `right: 0;`
*  `width: 300px;`
*  `border: 3px solid #73AD21;}`

**position: absolute**
An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).
However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.
> Note: A "positioned" element is one whose position is anything except static.
* `Example`
* `div.relative {`
*  `position: relative;`
*  `width: 400px;`
*  `height: 200px;`
*  `border: 3px solid #73AD21;}`
* `div.absolute {`
*  `position: absolute;`
*  `top: 80px;`
*  `right: 0;`
*  `width: 200px;`
*  `height: 100px;`
*  `border: 3px solid #73AD21;}`

**position: sticky**
An element with position: sticky; is positioned based on the user's scroll position.
A sticky element toggles between relative and fixed, depending on the scroll position. It is positioned relative until a given offset position is met in the viewport - then it "sticks" in place(like position:fixed).
* `Example`
* `div.sticky {`
*  `position: -webkit-sticky; /* Safari */`
*  `position: sticky;`
*  `top: 0;`
*  `background-color: green;`
*  `border: 2px solid #4CAF50;}`

**Overlapping Elements**
When elements are positioned, they can overlap other elements.
The z-index property specifies the stack order of an element (which element should be placed in front of, or behind, the others).
* An element can have a positive or negative stack order:
* `Example`
* `img {`
*  `position: absolute;`
*  `left: 0px;`
*  `top: 0px;`
*  `z-index: -1;}`
![Overlapping Elements](https://i.ytimg.com/vi/09wolz1jaqE/maxresdefault.jpg)


**Summary**

* `<div>` elements are often used as containing elements
to group together sections of a page.
* Browsers display pages in normal flow unless you
specify relative, absolute, or fixed positioning.
* The float property moves content to the left or right
of the page and can be used to create multi-column
layouts. (Floated items require a defined width.)
* Pages can be fixed width or liquid (stretchy) layouts.
* Designers keep pages within 960-1000 pixels wide,
and indicate what the site is about within the top 600
pixels (to demonstrate its relevance without scrolling).
* Grids help create professional and flexible designs.
* CSS Frameworks provide rules for common tasks.
* You can include multiple CSS files in one page.
