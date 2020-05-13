# Read: 05 - HTML Images; CSS Color & Text

## Images:
HTML Images Syntax
In HTML, images are defined with the `<img>` tag.
The `<img>` tag is empty, it contains attributes only, and does not have a closing tag.
The src attribute specifies the URL (web address) of the image: `<img src="url">`
**The alt Attribute**
The alt attribute provides an alternate text for an image, if the user for some reason cannot view it (because of slow connection, an error in the src attribute, or if the user uses a screen reader).
If a browser cannot find an image, it will display the value of the alt attribute.
The value of the alt attribute should describe the image:
* Example
* `<img src="img_chania.jpg" alt="Flowers in Chania">`
### Image Size - Width and Height
* You can use the style attribute to specify the width and height of an image.
* Example
* <`img src="img_girl.jpg" alt="Girl in a jacket" style="width:500px;height:600px;">`
* Alternatively, you can use the width and height attributes:
* Example
* `<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">`
* The width and height attributes always define the width and height of the image in pixels.

> Note: Always specify the width and height of an image. If width and height are not specified, the page might flicker while the image loads.

### Image as a Link
* To use an image as a link, put the `<img>` tag inside the `<a>` tag:
* Example
* `<a href="default.asp">`
*  `<img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;border:0;">`
* `</a>`

> Note: border:0; is added to prevent IE9 (and earlier) from displaying a border around the image (when the image is a link).

### Image Floating
* Use the CSS float property to let the image float to the right or to the left of a text:
* Example
* `<p><img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">`
* The image will float to the right of the text.`</p>`
* `<p><img src="smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">`
* The image will float to the left of the text.`</p>`

### HTML Screen Readers
* A screen reader is a software program that reads the HTML code, converts the text, and allows the user to "listen" to the content. Screen readers are useful for people who are visually impaired or learning disabled.
**Chapter Summary**
* Use the HTML `<img>` element to define an image
* Use the HTML src attribute to define the URL of the image
* Use the HTML alt attribute to define an alternate text for an image, if it cannot be displayed
* Use the HTML width and height attributes to define the size of the image
* Use the CSS width and height properties to define the size of the image (alternatively)
* Use the CSS float property to let the image float
* Loading images takes time. Large images can slow down your page. Use images carefully.

## HTML Colors
* Color Names In HTML, a color can be specified by using a color name
* Background Color You can set the background color for HTML elements
* `h1 style="background-color:DodgerBlue;">Hello World</h1>`

### Border Color
* `<h1 style="border:2px solid Tomato;">Hello World</h1>`

### Color Values
In HTML, colors can also be specified using RGB values, HEX values, HSL values, RGBA values, and HSLA values:

### RGB Color Values
* In HTML, a color can be specified as an RGB value, using this formula:
* rgb(red, green, blue)
* Each parameter (red, green, and blue) defines the intensity of the color between 0 and 255.
* This makes 256 x 256 x 256 = 16777216 possible colors!
* For example, rgb(255, 0, 0) is displayed as red, because red is set to its highest value (255) and the others are set to 0.
* To display black, set all color parameters to 0, like this: rgb(0, 0, 0).
* To display white, set all color parameters to 255, like this: rgb(255, 255, 255).

### RGBA Color Values
* RGBA color values are an extension of RGB color values with an alpha channel - which specifies the opacity for a color.
* An RGBA color value is specified with:
* rgba(red, green, blue, alpha)
* The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all)

### HEX Color Values
* In HTML, a color can be specified using a hexadecimal value in the form: #rrggbb
* Where rr (red), gg (green) and bb (blue) are hexadecimal values between 00 and ff (same as decimal 0-255).
* For example, #ff0000 is displayed as red, because red is set to its highest value (ff) and the others are set to the lowest value (00).

### HSL Color Values
* In HTML, a color can be specified using hue, saturation, and lightness (HSL) in the form:
hsl(hue, saturation, lightness)
* Hue is a degree on the color wheel from 0 to 360. 0 is red, 120 is green, and 240 is blue.
* Saturation is a percentage value, 0% means a shade of gray, and 100% is the full color.
* Lightness is also a percentage, 0% is black, 50% is neither light or dark, 100% is white

**Saturation**
* Saturation can be described as the intensity of a color.
* 100% is pure color, no shades of gray
* 50% is 50% gray, but you can still see the color.
* 0% is completely gray, you can no longer see the color.

**Lightness**
> The lightness of a color can be described as how much light you want to give the color, where 0% means no light (black), 50% means 50% light (neither dark nor light) 100% means full lightness (white).

### HSLA Color Values
* HSLA color values are an extension of HSL color values with an alpha channel - which specifies the opacity for a color.
* An HSLA color value is specified with:
* hsla(hue, saturation, lightness, alpha)
* The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all)

## Text
### Text Color
* The color property is used to set the color of the text. The color is specified by:
* a color name - like "red"
* a HEX value - like "#ff0000"
* an RGB value - like "rgb(255,0,0)"
* Look at CSS Color Values for a complete list of possible color values.
* The default text color for a page is defined in the body selector.
* Example
* `body {  color: blue;}`
* `h1 { color: green;}`

### Text Color and Background Color
* `body {`
* ` background-color: lightgrey;`
*  `color: blue;}`



properity |  Description
---------|---------
 `text-align` | property is used to set the horizontal alignment of a text. A text can be left or right aligned, centered, or justified.
 `direction` and `unicode-bidi` properties can be used to change the text direction of an element
 `vertical-align`|  property sets the vertical alignment of an element. This example demonstrates how to set the vertical alignment of an image in a text
`text-decoration`|  property is used to set or remove decorations from text.
 `text-transform`| property is used to specify uppercase and lowercase letters in a text. It can be used to turn everything into uppercase or lowercase letters, or capitalize the first letter of each word
 `text-indent`   |  property is used to specify the indentation of the first line of a text
 `letter-spacing`|  property is used to specify the space between the characters in a text. The following example demonstrates how to increase or decrease the space between characters
 `line-height`   |  property is used to set or remove decorations from text.
 `word-spacing`  |  property is used to specify the space between the words in a text.
 `white-space`   |  property specifies how white-space inside an element is handled.
 `text-shadow`   |  property adds shadow to text. In its simplest use, you only specify the horizontal shadow (2px) and the vertical shadow (2px).



   
  
