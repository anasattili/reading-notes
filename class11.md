# Read: 11 - Assorted Topics

## Images
**Controlling the size of image in css**
* `img {`
*    `max-width:100%;`
*    `height:auto;}`

**Controlling the Align of Image in css**
* `img.align-left {`
* `float: left;`
* `margin-right: 10px;}`
* `img.align-right {`
* `float: right;`
* `margin-left: 10px;}`
* `img.medium {`
* `width: 250px;`
* `height: 250px;}`

**Background-Imagies**
* `body { background-image: url("images/pattern.gif");}`

**Reapeated Imagies**
* `body {`
* `background-image: url("images/header.gif");`
* `background-repeat: repeat-x;}`

## Summary:
* you can specify the dimensions of  images using CSS.
This is very helpful when you use the same sized
images on several pages of your site.
* Images can be aligned both horizontally and vertically
using CSS.
* You can use a background image behind the box
created by any element on a page.
* Background images can appear just once or be
repeated across the background of the box.
* you can create image rollover effects by moving the
background position of an image.
* To reduce the number of images your browser has to
load, you can create image sprites.

## Practical Information

* Search engine optimization helps visitors find your
sites when using search engines.
* Analytics tools such as Google Analytics allow you to
see how many people visit your site, how they find it,
and what they do when they get there.
* To put your site on the web, you will need to obtain a
domain name and web hosting.
* FTP programs allow you to transfer files from your
local computer to your web server.
* Many companies provide platforms for blogging, email
newsletters, e-commerce and other popular website
tools (to save you writing them from scratch).

![SEO ](https://cdn.shortpixel.ai/client/q_glossy,ret_img/https://impideas.com/wp-content/uploads/2019/04/search-engine-optimization-seo-500x500.gif)

# Flash, Video & Audio:
> Flash is a very popular technology used
to add animations, video, and audio to
websites. We then focus on how to add video and audio to your site,
using either the new HTML5 `<video>` and `<audio>` elements
or a hosted service (such as YouTube or SoundCloud).

**How Flash works in web page**
> Flash Embedded in HTML
After creating a Flash movie you choose File > Save As from the top menu to save your movie. Save the file as "Somefilename.fla". 

* To embed the Flash movie you just made into an HTML page, you should go back to your Flash program and do the following steps:

* Step 1
Choose File > Open. Open a Flash movie you have created.
* Step 2
Choose File > Export Movie.
* Step 3
Name the file "somefilename.swf". Choose the location where the file is to be stored (in your Web folder). Click OK.
* Step 4
Open the HTML page where you want to insert your Flash movie. Insert this code:

* `code:`
* `<object width="550" height="400">`
* `<param name="movie" value="somefilename.swf">`
* `<embed src="somefilename.swf" width="550" height="400">`
* `</embed>`
* `</object>`

> Note: This is the minimum code you need to embed a Flash movie in a browser. A broken icon will appear on the Web page if the user does not have the Flash plug-in installed.

Note: In the code above there is both an `<embed>` tag and an `<object>` tag. This is because the `<object>` tag is recognized by Internet Explorer, and Netscape recognizes the `<embed>` tag and ignores the `<object>` tag.

* Step 5
Type in the address of the HTML file in your browser and look at your first Flash movie.


Let the Flash Program do the Work.
The code above is the absolute minimum code to embed Flash movies in HTML pages. It is not recommended to use the minimum code. There should be a few more attributes added:
classid is an attribute to the `<object>` tag. It tells Internet Explorer to load the ActiveX plug-in if it is not installed
pluginspage is an attribute to the `<embed>` tag. It displays a link to the Shockwave download page if Netscape does not have it 


* The Flash program can add these attributes for you:

* Step 1
Choose File > Publish. Flash will now create the <object>, <param>, and <embed> tags for you. It will also create the classid and pluginspage attributes.
* Step 2
Open the HTML document that Flash created, view the HTML source and copy the code into your HTML page where you want your Flash movie.
* Step 3
Be sure that you have the "somefilename.swf" in your Web folder.
* Step 4
Type in the address of the HTML file in your browser and look at your first Flash movie.




