<!-- experimenting with styling options -->

<head>
  <style>
    code {
      color: green;
    }
  </style>
</head>

### Class 03 Reading Notes

## HTML List Tags

<table>
  <tr>
    <th>tag</th>
    <th>usage</th>
  </tr>
  <tr>
    <td><code>&lt;ol&gt;&lt;/ol&gt;</code></td>
    <td>ordered list</td>
  </tr>
  <tr>
    <td><code>&lt;ul&gt;&lt;/ul&gt;</code></td>
    <td>unordered list</td>
  </tr>
  <tr>
    <td><code>&lt;li&gt;&lt;/li&gt;</code></td>
    <td>list item</td>
  </tr>
  <tr>
    <td><code>&lt;dl&gt;&lt;/dl&gt;</code></td>
    <td>definition list, for a series of terms and their definitions</td>
  </tr>
  <tr>
    <td><code>&lt;dt&gt;&lt;/dt&gt;</code></td>
    <td>definition term, placed inside <code>&lt;dl&gt;</code> tags </td>
  </tr>
  <tr>
    <td><code>&lt;dd&gt;&lt;/dd&gt;</code></td>
    <td>definition definition, placed inside <code>&lt;dl&gt;</code> tags, after a <code>&lt;dt&gt;</code> tag</td>
  </tr>
</table>

## HTML Nested List Example

code:

<!-- referenced https://www.w3schools.com/tags/tag_pre.asp -->
<pre>
<code style="color: green;">
&lt;ul&gt;
  &lt;li&gt;list item 1&lt;/li&gt;
  &lt;li&gt;list item 2&lt;/li&gt;
    &lt;ul&gt;
      &lt;li&gt;list item a&lt;/li&gt;
      &lt;li&gt;list item b&lt;/li&gt;
    &lt;/ul&gt;
  &lt;li&gt;list item 3&lt;/li&gt;
&lt;/ul&gt;
</code>
</pre>

result:

<ul>
  <li>list item 1</li>
  <li>list item 2</li>
    <ul>
      <li>list item a</li>
      <li>list item b</li>
    </ul>
  <li>list item 3</li>
</ul>

## CSS Box Controls

<table>
  <tr>
    <th>properties</th>
    <th>usage</th>
    <th>value example</th>
  </tr>
  <tr>
    <td><code>width<br />height</code></td>
    <td>controls dimensions</td>
    <td>
      <ul>
        <li>300px</li>
        <li>80%</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><code>min-width<br />min-height<br />max-width<br />max-height</code></td>
    <td>controls minimum/maximum dimensions</td>
    <td>
      <ul>
        <li>300px</li>
        <li>80%</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><code>overflow</code></td>
    <td>controls content in box that is too large to fit</td>
    <td>
      <ul>
        <li>hidden</li>
        <li>scroll</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><code>border</code></td>
    <td>controls the edge of the box</td>
    <td>
    </td>
  </tr>
  <tr>
    <td><code>border-width</code></td>
    <td>controls border thickness</td>
    <td>
      <ul>
        <li>2px</li>
        <li>thick</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><code>border-style</code></td>
    <td>controls border type</td>
    <td>
      <ul>
        <li>solid</li>
        <li>ridge</li>
        <li>hidden</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><code>border-color</code></td>
    <td>controls border color</td>
    <td>
      <ul>
        <li>#ffffff</li>
        <li>rgb(255, 255, 255)</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><code>padding</code></td>
    <td>controls space between the border and the content inside the box</td>
    <td>
      <ul>
        <li>10px</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><code>margin</code></td>
    <td>controls space outside the border</td>
    <td>
      <ul>
        <li>10px</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><code>text-align</code></td>
    <td>controls alignment of content in box, it is inherited so you can override it in the content tag</td>
    <td>
      <ul>
        <li>center</li>
        <li>left</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><code>display</code></td>
    <td>allows adjusting/switching behavior of block and inline elements</td>
    <td>
      <ul>
        <li>inline</li>
        <li>block</li>
        <li>inline-block</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td><code>visibility</code></td>
    <td>controls visibility</td>
    <td>
      <ul>
        <li>hidden</li>
        <li>visible</li>
      </ul>
    </td>
  </tr>
</table>

## JS Do While Loop

A do while loop acts just like a while loop except it runs the code once without checking the condition. (the condition is at the end instead of the start). So even if the condition is false, like below, it will still execute the code once.

```
do {
  this thing once;
} while (false);
```

or

```
do {
  this thing then check the condition before doing again;
} while (condition);
```

[Return to table of contents](../README.md)