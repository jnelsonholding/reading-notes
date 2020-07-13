<head>
  <style>
    code {
      color: green;
    }
  </style>
</head>

### Class 06 Reading Notes

<h1 id="jsobjects"></h1>

## JavaScript Objects

Objects are a way of grouping variables and functions to create models. When a variable belongs to an object, it's referred to as a *property*. Similarly, when a function belongs to an object, it's called a *method*.

For example, a dog named Lassie might have these properties (characteristics):

<pre><code style="color: green;">
lassie.name; // 'Lassie'
lassie.color; // ['black', 'white', 'sable']
lassie.goodTemper; // true
</code></pre>

And Lassie might also have these methods (actions):

<pre><code style="color: green;">
lassie.bork(); // barks
lassie.timmyFellDownWell(); // barks at Pa
</code></pre>

Creating the object *lassie* might look like this:

<pre><code style="color: green;">
var lassie = {
  name : 'Lassie',
  color : ['black', 'white', 'sable'],
  goodTemper : true,
  bork: function() {
    console.log('bark');
  },
  timmyFellDownWell: function() {
    console.log('Hey Pa!');
    lassie.bork();
  }
};
</code></pre>

Side note - apparently Timmy never fell down a well. I guess Lassie did.

<h1 id="jsdocument"></h1>

## JavaScript Document Object Model

The document object contains the tree of nodes that make up a web page, including the html node, so everything. Each node is actually an object as well. And the document object has a variety of methods to help access the nodes so you can change their properties.

<table>
  <tr>
    <th>method/example</th>
    <th>usage</th>
  </tr>
  <tr>
    <td><code>document.getElementById('puppyImg')</code></td>
    <td>returns the object node for the element with its attribute <code>id="puppyImg"</code></td>
  </tr>
  <tr>
    <td><code>document.querySelector('div.cheese')</code></td>
    <td>returns the object node for the first element targeted by the CSS selector <code>div.cheese</code></td>
  </tr>
  <tr>
    <td><code>document.getElementsByClassName('cheese')</code></td>
    <td>returns a nodelist (like an array) of object nodes for elements with the attribute <code>class="cheese"</code></td>
  </tr>
  <tr>
    <td><code>document.getElementsByTagName('h1')</code></td>
    <td>returns a nodelist of object nodes for <code>h1</code> elements</td>
  </tr>
  <tr>
    <td><code>document.querySelectorAll('div.cheese')</code></td>
    <td>returns a nodelist of object nodes for all <code>div</code> elements with the attribute <code>class="cheese"</code></td>
  </tr>
  <tr>
    <td><code>element.parent()</code></td>
    <td>returns the object node for the parent of the element object</td>
  </tr>
  <tr>
    <td><code>element.firstChild()</code><br /><code>element.lastChild()</code></td>
    <td>returns the first or last child of the element</td>
  </tr>
  <tr>
    <td><code>element.previousSibling()</code><br /><code>element.nextSibling()</code></td>
    <td>returns the previous or next sibling of the element</td>
  </tr>
</table>

The last two examples can be difficult to manage. Other than IE, browsers will return white space as sibling elements as if they are text nodes.

[Return to table of contents](../README.md)

