<head>
  <style>
    code {
      color: green;
    }
  </style>
</head>

### Class 07 Reading Notes

<h1 id="htmltables"></h1>

## HTML Tables

<table>
  <tr>
    <th>tags</th>
    <th>usage</th>
  </tr>
  <tr>
    <td><code>&lt;table>&lt;/table></code></td>
    <td>the main table element, filled with rows</td>
  </tr>
  <tr>
    <td><code>&lt;tr>&lt;/tr></code></td>
    <td>table row, wraps the cells for each row</td>
  </tr>
  <tr>
    <td><code>&lt;th>&lt;/th></code></td>
    <td>table header, contains the content for header cells</td>
  </tr>
  <tr>
    <td><code>&lt;td>&lt;/td></code></td>
    <td>table data, contains the content for data cells</td>
  </tr>
  <tr>
    <td><code>&lt;td colspan="2">&lt;/td></code></td>
    <td>column span, this attribute allows a cell to stretch across multiple columns, in this case 2 columns</td>
  </tr>
  <tr>
    <td><code>&lt;td rowspan="3">&lt;/td></code></td>
    <td>row span, this attribute allows a cell to stretch down over multiple rows, in this case 3 rows</td>
  </tr>
  <tr>
    <td><code>&lt;thead>&lt;/thead></code></td>
    <td>table head, for long tables, surrounds the <code>&lt;tr></code> and <code>&lt;th></code> elements</td>
  </tr>
  <tr>
    <td><code>&lt;tbody>&lt;/tbody></code></td>
    <td>table body, for long tables, surrounds the <code>&lt;tr></code> and <code>&lt;td></code> elements that comprise the data</td>
  </tr>
  <tr>
    <td><code>&lt;tfoot>&lt;/tfoot></code></td>
    <td>table footer, for long tables, surrounds the <code>&lt;tr></code> and <code>&lt;td></code> elements that comprise the summary, likely for totals for the data in the <code>&lt;tbody></code></td>
  </tr>
</table>

<h1 id="jsobjects"></h1>

## JavaScript Objects

Another way to declare an object is by using the `new` keyword and `Object()` constructor function.

<pre><code style="color: green;">
var lassie = new Object();
lassie.name = 'Lassie';
lassie.color = ['black', 'white', 'sable'];
lassie.goodTemper = true;
lassie.bork = function() {
  console.log('bark');
};
lassie.timmyFellDownWell = function() {
  console.log('Hey Pa!');
  lassie.bork();
};
</code></pre>

When accessing properties, an alternative to dot notation is using square brackets:

`lassie['name'] = 'Lassie';`

But wait, why make a unique object every time when there are so many similarities between them? You can just make your own object constructor function! Note that convention dictates the name of an object constructor starts with a capital letter, so get your pinky on that shift key.

<pre><code style="color: green;">
function Dog(name, color, goodTemper) {
  this.name = name;
  this.color = color;
  this.goodTemper = goodTemper;
  this.bork = function() {
    console.log('bark');
  };
}
</code></pre>

Now we can make as many dog objects as we want!

<pre><code style="color: green;">
var lassie = new Dog('Lassie', ['black', 'white', 'sable'], true);
var lancer = new Dog('Lancer', ['neon green'], false);
</code></pre>

These dogs' properties are set through the constructors parameters. And they can both bork!

Notice the use of `this` when creating a constructor. `this` basically means "this object". So when this.bork() is called inside lassie, it essentially becomes lassie.bork(). Which is really useful because it does the same thing for lancer. Otherwise, calling for lancer to bork() might end up causing lassie to bark.

<h1 id="builtin"></h1>

## JavaScript Built-In Objects

There are three groups of built-in objects; Browser Object Model, Document Object Model, and Global JavaScript Objects.

The main object in the Browser Object Model is the Window object. Its properties reference useful details about the browser itself and things like screen width.

The Document Object Model represents the web page. Basically the document object covers everything in the html. This allows targeting and manipulating of elements.

Global objects are things like data types. Strings have all sorts of built in methods that allow changing cases or cutting parts of the string out. Numbers as well. Something that is pretty handy is the `isNaN()` method to check if something is not a number.

The Math object is built into JavaScript to allow for mathematical operations like rounding and retrieving a random number.

The Date object allows getting and setting dates and times.

[Return to table of contents](../README.md)

