# Read: 01 - Introductory HTML and JavaScript

## How People Access the Web:
* Browsers: it’s a software called web browsers to view the web pages.
* web servers: a special computer respond to the request of the users.
* devices: the end users’ devices like laptop tablets mobiles.
* screen reader: a software which read the content of the computer screen.

**The basic web pages created by using HTML and CSS.**

## How the web works:
> connect to the internet by (ISP) by write the name of the web page on browser
DNS server convert the name to the unique IP address to contact you with the web server
the web server sends the page you request to your web browser.

## HTML: is a hypertext markup language, used to build the structure of the web pages.
### the structure of the web pages using html:
the structure of the web pages using html
`<!DOCTYPE>`.........declaration the html.
`<html>`......contain the html element.
`<head> <title>`.......to add a title for the web page tab.
`<body>`............contain all the visible element of the web pages.
//body can contain: header, paragraph, main, section, article, footer......//
open tag like`<html>` to indicate the tag's purpose.
close tag like`</html>` to indicate the end of the tag action.
Attributes: using in the open tag to provide additional information
about the contents of an element. ex:`<p lang="en-us">Paragraph in English</p>.`

versions of HTML.
HTML4-XHTML 1.0-HTML5
TO use each of them depending on the first tag of the declaration. ex:`<!doctype html>` for html5.

Comments on HTML:
`<!-- comment goes here -->`
add a comment to your code it’s a good idea to you when you return back to fix some problems make it easy or for if someone else needs to look at the code.

Id Attribute: The HTML id attribute is used to specify a unique id for an HTML element (the value must be unique within the HTML document).
ex: `<h1 id="myHeader">My Header</h1>.`

Class Attribute: The HTML class attribute is used to define equal styles for elements with the same class name.
ex: 
  `<h2 class="cities">London</h2>`
  `<h2 class="cities">Paris</h2>`

 Element   |  Function
-----------|-----------
`<div>`    | allows you to group a set of elements together in one block-level box.
`<span>`   |to contain a text or a number of inline element and the most use of it to control the appearance of the content of these elements using CSS.
`<iframe>` | allows you to group a set of elements together in one block-level box.
`<meta>`   |  >:is a data (information) about data. And its invisible element. meta tags always go inside the head element, and they provide metadata about the HTML document. meta tags are typically used to specify character set, page description, keywords, author of the document, and viewport settings.
`<header>` | element represents a container for introductory content or a set of navigational links.
`<footer>` | element typically contains: authorship information, copyright information, contact information.
`<nav>`    | element represents a section of a page whose purpose is to provide navigation links, either within the current document or to other documents. Common examples of navigation sections are menus, tables of contents, and indexes.
`<article>`| Represents a self-contained composition in a document, page, application, or site, which is intended to be independently distributable or reusable. Examples include: a forum post, a magazine or newspaper article, or a blog entry.
`<aside>`  | Represents a portion of a document whose content is only indirectly related to the document's main content. Asides are frequently presented as sidebars or call-out boxes.
`<section>`|  element represents a standalone section — which doesn't have a more specific semantic element to represent it — contained within an HTML document. Typically, but not always, sections have a heading.
`<hgroup>` | Represents a multi-level heading for a section of a document. It groups a set of `<h1>–<h6>` elements.
`<figure>and<figcaption>` | represents self-contained content, potentially with an optional caption, which is specified using the `(<figcaption>)` element. The figure, its caption, and its contents are referenced as a single unit.

## Process & Design
### Criteria’s for build a website for Individuals:
* Age
* Gender
* Location
* Occupation
* Income
* Web use(time)
### Criteria’s for build a website for Companies:
* The size of company
* The position of people in the company
* The way of using of people in company for themselves or for someone else
* The budget

> People visit your site depend on their motivations and goals. using sitemap and wireframes to organize the web page.


## Visual Hierarchy:
 > using to specifying some Key world or text to helps users find what they are looking for by control the(size-color-style-images)

## Grouping and Similarity: 
> organize visual elements into groups. Grouping related pieces of information together can make a design easier to comprehend.
ex:(proximity-closure-continuance-white space-color-border)

## Designing Navigation: 
> TO help users understand about the site and organize it and where users want to go.
characteristics of good navigation bar: (concise-clear-selective-context-interactive-consistent).


## JavaScript:
### is a programming language allowing you to make the web pages more interactive by using this characteristics:
Access content: ex: select the text inside all of `<h1>`.
Modify content: ex: change the size or position of image.
Program rules: ex: action applied depending on condition of loop.
React to event: ex: a button is pressed.

## The ABC of Programming:
Script: is a series of instructions that a computer can follow to achieve a goal. Like recipes or manuals.
Writing a script:
-define the goal
-design the script
-code each step
To start write the code you should know the vocabulary and syntax of the language and breaks the scripts into small tasks.
When you try to write the instruction for computer(code). you should use another way from ask a person to do in. Because computer can't understand the way which people 
communicate you should convert it as a step of instructions in a correct logical order to make computer understand it. You can use flow chart for each step to make it easy.

**The computer understands the physical things like car, hotel, park as an object.**

### The object has three main point:
* properties: the names and values of the object ex: the color of the car.
* event: when users interact with the object in the web page. ex: press a button.
* method: occur after the event and it done without need to understand from users. ex: after press a button there is a block of instruction done to make the change.

### How browser see the web page:
* The browsers receive the html page
* Creates a model of the page and stores it in memory
* Show page on screen using rendering engine  

### How HTML, CSS, and JavaScript fit together:
* First HTML give the structure for the element of the web page
* Second CSS enhances the HTML page with rules that state how the HTML content is presented
* Third JavaScript can change how the page behaves, and make the page more interactive with users.

> The best practice is to keep the three languages in separate files, with the HTML page linking to CSS and JavaScript files.



















