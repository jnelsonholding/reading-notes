<head>
  <style>
    code {
      color: green;
    }
  </style>
</head>

### Class 04 Reading Notes

## HTML Links

Links are wrapped in the `<a></a>` tag. Text placed between those tags shows up as the clickable text for a link on the page.

The magic of the link is in the `href` attribute, which has the address value that tells the browser where to go. Here are some usage examples:

<table>
  <tr>
    <th>href</th>
    <th>result</th>
  </tr>
  <tr>
    <td><code>href="http://google.com"</code></td>
    <td>sends user to google, an external site</td>
  </tr>
  <tr>
    <td><code>href="about.html"</code></td>
    <td>sends user to the "about" page of the same site, if the "about" page is in the same directory</td>
  </tr>
  <tr>
    <td><code>href="../movies/listing.html"</code></td>
    <td>sends user to a page on the same site, file is located up one directory and then in the movies folder compared to the current page</td>
  </tr>
  <tr>
    <td><code>href="#contactInfo"</code></td>
    <td>scrolls the user's browser view to the html element with the attribute <code>id="contactInfo"</code></td>
  </tr>
  <tr>
    <td><code>href="mailto:jnelson.java@gmail.com"</code></td>
    <td>opens user's default email client and inserts jnelson.java@gmail.com into "to" address</td>
  </tr>
</table>

If you want the link to open in a new window instead of navigating away from your page, use the attribute `target="_blank"`.

## CSS Layout

### Positioning

Note that anything that is removed from normal flow will risk overlapping.

<table>
  <tr>
    <th>type</th>
    <th>code</th>
    <th>description</th>
  </tr>
  <tr>
    <td>normal flow</td>
    <td><code>position: static;</code></td>
    <td>default, each block-level element sits on top of the next</td>
  </tr>
  <tr>
    <td>relative position</td>
    <td><code>position: relative;</code></td>
    <td>removed from normal flow, moves relative to the position it would naturally be in normal flow</td>
  </tr>
  <tr>
    <td>absolute positioning</td>
    <td><code>position: absolute;</code></td>
    <td>removed from normal flow, position is relative to its container</td>
  </tr>
  <tr>
    <td>fixed positioning</td>
    <td><code>position: fixed;</code></td>
    <td>removed from normal flow, position relative to the browser window, like those things that stay in the middle of your screen even though you're scrolling</td>
  </tr>
</table>

Probably gonna have some instances where things overlap. Use `z-index: 5;` to indicate which element should be on top. The higher the index number, the higher its visual priority.

`float` will move an element as far to the left or right of its container as possible. Anything else in the container will flow around the floated element.

A container with only floated elements can have an issue where it appears as a line. In order to give it dimensions, try these two properties: `overflow: auto;` and `width: 100%;`.

Note that variable screen sizes are a major consideration when designing a page. Designers often make their pages aroudn 960px-1000px as most screens will display that naturally.

## JavaScript Functions

Basic way to declare and call a function:

<pre>
<code style="color: green;">
function doTheThing(parameter1, parameter2) {
  // do the thing using parameter variables;
  // possibly return a thing;
}

doTheThing(parameter1 = argument1, parameter2 = argument2);
// or
doTheThing(argument1, argument2);
</code>
</pre>

or using a function expression with an anonymous function:

<pre>
<code style="color: green;">
var doTheThing = function(parameter1, parameter2) {
  // do the thing using parameter variables;
  // possibly return a thing;
}

doTheThing(parameter1 = argument1, parameter2 = argument2);
// or
doTheThing(argument1, argument2);
</code>
</pre>

[Return to table of contents](../README.md)
































