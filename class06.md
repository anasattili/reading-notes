# Read: 06 - JS Object Literals; The DOM

## Object Literals:
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.

### Property:
 Properties te ll us about the object, such as
the name of a hotel or the number of rooms it has.

###  Method:
Methods represent tasks that are associated with
the object.

### Creating an object (literal notation):
> Literal notaion is the most and easy way to create objects.

### Accessing an object and dot notation:
> access the properities and methods of an object using dot notation.
You can access properities by using square brackets.

`Example:`
`var hotel = {`
`name: 'Quay',`
`rooms : 40,`
`booked: 25,`
`checkAvailability: function() {`
`return this.rooms - this.booked;`
`}`
`} ;`
`JAVASCRIPT`
`var elName = document .getElementByld('hotelName');`
`elName.textContent =hotel .name;`
`var elRooms = document.getElementByid{'rooms');`
`elRooms .textContent = hotel .checkAvailability();`

## Document Object Model
> The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

**Making A Model of the HTML page**
 When the browser loads a web page, it creates a model of the page in memory.

**Accessing and changing the HTML page**

> The DOM also defines methods and properties to access and update each object in this model, which in turn updates what the user sees in the browser. You will hear people call the DOM an Application Programming Interface (API). User interfaces let humans interact with programs; APls let programs (and scripts) talk to each other.

## The DOM Tree is a Model of a Web Page
As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.

![DOM Tree](https://www.researchgate.net/profile/Jian_Chang4/publication/254002847/figure/fig1/AS:298235726974978@1448116346303/Example-of-DOM-Node-Tree.png)

**changing dom quiries**
grtelementbyId('one');

**Accessing Elemeny**
`getElementByld(id);`
`querySel ector( 'css selector ');`
`getEl ement sByClassName( 'class ');`
`getEl ementsByTagName( ' tagName ');`
`querySelectorAll ( 'css select');`

**Method select individual element**
document.getElementById('id');

### NODELISTS: DOM QUERIES
THAT RETURN MORE THAN ONE ELEMENT When a DOM method can return more than one element, it returns a Nodelist (even if it only finds one matching element).

### Selecting and elements from a nodelists
`nodeItem = nodeList.item(index);` 
> nodeList is a NodeList. This is usually obtained from another DOM property or method, such as childNodes.
index is the index of the node to be fetched. The index is zero-based. nodeItem is the indexth node in the nodeList returned by the item method.

### select elements using class attribute
`var elements = document .getEl ementsByClassName('class');`

### select elements using a tag name
`var elements = document.getElementsByTagName('li ');`

### select element using CSS selectore
`var la = document .querySel ector('li .red ' };`

### Looping through a nodelist
`var hotltems = document .querySelectorAl l (' l i . hot') ; // Store Nodel i st in ar ray`
`if (hot ltems.length > O) { // If it contains items`
`for (var i=O; i<hotl tems.length; i++) { // Loop through each item`
`hotltems[i ] .className = 'cool'; // Change value of class attribute} }`

### Traversing the dom
![Traversing the dom](https://www.qualitestgroup.com/images/howto/DOMTree_HowTo.png)

### ACCESS & UPDATE A TEXT NODE WITH NODEVALUE
document.getElementByid( 1 one 1 ).firstChild.nextSibling. nodeValue;
\       step one                  \ step 2   \ step 3    \ step 4   \ 

### Adding and removing HTML content
**Creating New HTML Elements (Nodes)**
To add a new element to the HTML DOM, you must create the element (element node) first, and then append it to an existing element.

 `Example`
`<div id="div1">`
  `<p id="p1">This is a paragraph.</p>`
  `<p id="p2">This is another paragraph.</p>`
`</div>`
`<script>`
`var para = document.createElement("p");`
`var node = document.createTextNode("This is new.");`
`para.appendChild(node);`
`var element = document.getElementById("div1");`
`element.appendChild(para);`
`</script>`

**Removing Existing HTML Elements**
To remove an HTML element, use the `remove()` method:
`Example`
`<div>`
  `<p id="p1">This is a paragraph.</p>`
  `<p id="p2">This is another paragraph.</p>`
`</div>`
`<script>`
`var elmnt = document.getElementById("p1");`
`elmnt.remove();`
`</script>`

### Attributes node
`var firstitem = document.getElementByid( 'one');  // Get first list item`
`if (firstitem.hasAttribute('class')) {  // If it has class attribute`
`var attr = firstltem.getAttribute(' class');  // Get the attribute`
`// Add the value of the attribute after the list`
`var el = document .getElementByid( ' scriptResults');`
`el .innerHTML = '<p>The first i tem has a class name : ' + attr + '<Ip>';`

## SUMMARY About DOM:
* The browser represents the page using a DOM tree.
* DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes.
* You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax.
* Whenever a DOM query can return more than one node, it will always return a Nadel i st.
* From an element node, you can access and update its  content using properties such as textContent and        content using properties such as textContent and i nnerHTML or using DOM manipulation techniques.    
* An element node can contain multiple text nodes and child elements that are siblings of each other.
* In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).
* Browsers offer tools for viewing the DOM tree .























