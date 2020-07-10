### Class 02 Reading Notes

<h1 id="htmltext"></h1>

## HTML Text Tags

<!-- experimenting with <code> tags found at http://web.simmons.edu/~grabiner/comm244/weekfour/code-test.html -->
<!-- doesn't do anything significant here because the text is already monospace, so I'm styling it -->
<table>
  <tr>
    <th>tag</th>
    <th>usage</th>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;h1&gt;&lt;/h1&gt;</code></td>
    <td>header, h1 through h6</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;p&gt;&lt;/p&gt;</code></td>
    <td>paragraph</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;b&gt;&lt;/b&gt;</code></td>
    <td>bold</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;i&gt;&lt;/i&gt;</code></td>
    <td>italic</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;sup&gt;&lt;/sup&gt;</code></td>
    <td>superscript</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;sub&gt;&lt;/sub&gt;</code></td>
    <td>subscript</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;br /&gt;</code></td>
    <td>line break</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;hr /&gt;</code></td>
    <td>horizontal rule (line to create visual separation</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;strong&gt;&lt;/strong&gt;</code></td>
    <td>indicates importance, default bold</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;em&gt;&lt;/em&gt;</code></td>
    <td>indicates emphasis, default italic</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;blockquote&gt;&lt;/blockquote&gt;</code></td>
    <td>used to wrap around larger or visually distinct quotes, still needs &lt;p&gt; tags around text and should use <i>cite</i> attribute to link source</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;q&gt;&lt;/q&gt;</code></td>
    <td>short or inline quote, also uses cite attribute to link source, <strong>note that this is not well supported by IE browsers so is generally avoided</strong></td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;abbr&gt;&lt;/abbr&gt;</code></td>
    <td>abbreviation or acronym</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;cite&gt;&lt;/cite&gt;</code></td>
    <td>denotes title of a book or other work, default italic</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;dfn&gt;&lt;/dfn&gt;</code></td>
    <td>definition, inconsistent default formatting across various browsers</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;address&gt;&lt;/address&gt;</code></td>
    <td>wraps contact info for webpage's author (that's you!)</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;ins&gt;&lt;/ins&gt;</code></td>
    <td>denotes inserted text, default underline</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;del&gt;&lt;/del&gt;</code></td>
    <td>denotes removed text, default strikethrough</td>
  </tr>
  <tr>
    <td><code style="color: green;">&lt;s&gt;&lt;/s&gt;</code></td>
    <td>strikethrough</td>
  </tr>
</table>

<h1 id="csspriority"></h1>

## CSS Priority and Inheritance

Certain properties are inherited by an element's children. For instance, a `font-family` property targeting the `<body>` element would also apply to a `<p>` element inside the body. This is a great feature to allow a cohesive style across a page without repetitive code.

To provide the opportunity to overrule a property, CSS will choose the more specific selector when there is conflict. In the previous example, a `<p>` element is a more specific target than a `<body>` element, so it would choose the `<p>` element's styling. Similarly, an ID selector is more specific than a type selector, so the ID specific value would overrule a conflicting property for the general type.

<h1 id="jsfun"></h1>

## Fun with JavaScript

JavaScript creates the action for a page. To make it go, you need to access the object that holds all of the page, the document object. Here are some examples of accessing a changing parts of the page:

```
/* uses the document object's getElementById() method to save an element with the ID 'header' in the variable h1WithIdHeader */

var h1WithIdHeader = document.getElementById('header');
```

```
/* the element stored in h1WithIdHeader is a node, an object, with a property 'textContent' which is now getting the string value 'new text' */

h1WithIdHeader.textContent = 'new text';
```

[Return to table of contents](../README.md)
