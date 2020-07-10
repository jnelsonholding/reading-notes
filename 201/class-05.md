<head>
  <style>
    code {
      color: green;
    }
  </style>
</head>

### Class 05 Reading Notes

<h1 id="htmlimages"></h1>

## HTML Images

Add images to a page using the `<img></img>` element. Specify the image using the `<img>` element's attributes:

<table>
  <tr>
    <th>attribute</th>
    <th>example</th>
    <th>usage</th>
  </tr>
  <tr>
    <td>src</td>
    <td><code>src="bunny.jpg"</code></td>
    <td>displays image contained in the file 'bunny.jpg'</td>
  </tr>
  <tr>
    <td>alt</td>
    <td><code>alt="A bunny mid hop"</code></td>
    <td>creates alternate text for the image if it can't be seen, good for accessibility</td>
  </tr>
  <tr>
    <td>title</td>
    <td><code>title="The domesticated bunny is an adorable household pet"</code></td>
    <td>creates a title that would usually display if the user hovers over the image</td>
  </tr>
</table>

Interesting note about image placement: `<img>` is an inline element. So if you place it inside a block level element like `<p>`, it will sit inside the text box with the bottom of the image aligned to the bottom of the text next to it.

<h1 id="csscolors"></h1>

## CSS Colors

The main color properties are `color`, for foreground color, and `background-color`, for background color. The values for these are `rgb(255, 255, 255)` where red, green, and blue are determined by numbers between 0 and 255. Or the same can be represented in hexadecimal: `#ffffff`, where each two digits represents a number between, you guessed it, 0 and 255. Also, some colors can be defined by name, like `green`.

The most recent browsers allow use of the `rgba` property, which is the same as the `rgb` property except it adds a fourth value known as the alpha. It controls the opacity of the color and is set with a value between 0.0 and 1.0. If you use this property, then it is best to also use `rgb` right before it so that if an older browser does not recognize `rgba`, it will revert to the `rgb` set on the previous line.

CSS3 has another feature that won't work on other browsers but give some more color flexibility. `hsl` stands for hue, saturation, lightness. Hue takes a value between 0 and 360, which represents a point on a color wheel. Saturation is the amount of gray and is set with a percentage where 100% is full color and 0% is a shade of gray. Lightness is the amount of white (lightness) or black (darkness) and is also set with a percentage where 100% is black, 50% is normal, and 0% is white.

`hsla` is the same as hsl except it adds alpha, a number between 0.0 and 1.0, representing transparency.

<h2 id="csstext"></h2>

## CSS Text

`font-family: Georgia, Times, serif;` sets the font and is inherited by sub-elements. If the browser doesn't have the first font available, `Georgia` in this example, it will move to the next, `Times`. It's best practice to end with a generic font family so the browser can use its default if it didn't have any fonts you specified.

`font-size: 1.3em;` sets the font size. It can be set by specifying pixels, `12px`, by a percentage relative to the default browser size, `75%`, or by relating it to the size of the parent element, `1.3em`.

You can specify a font even if the client doesn't have it by using `@font-face`. Because different browsers accept different font formats, you'll have to specify multiple. The order they should be specified in is:

  1. `.eot format('embedded-opentype')`
  1. `.woff format('woff')`
  1. `.ttf format('truetype')` (or .otf)
  1. `.svg format('svg')`

More text attributes:

<table>
  <tr>
    <th>attribute</th>
    <th>value examples</th>
    <th>description</th>
  </tr>
  <tr>
    <td><code>font-weight</code></td>
    <td><code>normal<br />bold</code></td>
    <td>creates bold text</td>
  </tr>  
  <tr>
    <td><code>font-style</code></td>
    <td><code>normal<br />italic<br />oblique</code></td>
    <td>creates italic text</td>
  </tr>  
  <tr>
    <td><code>text-transform</code></td>
    <td><code>uppercase<br />lowercase<br />capitalize</code></td>
    <td>adjusts the case</td>
  </tr>  
  <tr>
    <td><code>text-decoration</code></td>
    <td><code>none<br />underline<br />overline<br />line-through<br />blink</code></td>
    <td>adjusts decor, handy for making links look like links</td>
  </tr>  
  <tr>
    <td><code>line-height</code></td>
    <td><code>1.4em</code></td>
    <td>adjusts line height (space above a line of text, like text line margin-top)</td>
  </tr>  
  <tr>
    <td><code>letter-spacing</code></td>
    <td><code>0.2em</code></td>
    <td>adjusts space between letters (kerning)</td>
  </tr>  
  <tr>
    <td><code>word-spacing</code></td>
    <td><code>1em</code></td>
    <td>adjusts space between words</td>
  </tr>  
  <tr>
    <td><code>text-align</code></td>
    <td><code>left<br />right<br />center<br />justify</code></td>
    <td>aligns text</td>
  </tr>  
  <tr>
    <td><code>vertical-align</code></td>
    <td><code>baseline<br />sub<br />super<br />top<br />text-top<br />bottom</code></td>
    <td>seems to align text with another inline element</td>
  </tr>  
  <tr>
    <td><code>text-indent</code></td>
    <td><code>20px</code></td>
    <td>indents text, value can be negative and can indent the text off the screen</td>
  </tr>  
  <tr>
    <td><code>text-shadow</code></td>
    <td><code>1px<br />#111111</code></td>
    <td>creates ddrop shadow, takes 2 px values representing left/right and top/bottom drop, plus an optional 3<sup>rd</sup> px value for blur, and lastly a color</td>
  </tr>  
</table>

[Return to table of contents](../README.md)

