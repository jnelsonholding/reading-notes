### Notes on CSS

CSS contains two parts: a **selector** and a **declaration**.

- *selector*{*declaration*}

The declaration is made of two parts: a **property** and a **value**.

- {*property*: *value*;}

The link element sits in the head of the HTML and points to the .css stylesheet.

- `<link href="css/styles.css" type="test/css" rel="stylesheet" />`

### Color in CSS

The color and background-color properties have three types of values allowed:

- RGB Values: rgb(100,100,100) (red, green, blue) (numbers between 0 and 255)
- Hex Codes: #a1b2c3 (hexadecimal: 0 - f)
- Color Names: DarkCyan (note there are 147 specific colors with names)

For text to be legible, it's important to choose a color with enough contrast compared to the background-color.

A newer property is opacity. It allows you to make an HTML element transparent.

- {color: red; opacity: 0.5}
- opacity values are between 0.0 and 1.0

Also a newer property is *hsl*. It allows you to specify the hue, saturation, and lightness of an element with ease.

- hue is represented by numbers between 0 and 360.
- saturation is a percentage.
- lightness is a percentage where 0% is white and 100% is black.
- eg. {color: red; hsl(0, 10%, 50%)}

*hsla* is the same as hsl except it includes a 4th value: Alpha. Alpha is a number between 0.0 and 1.0 representing transparency.

[Return to table of contents](README.md)