<head>
  <style>
    code {
      color: green;
    }
  </style>
</head>

### Class 10 Reading Notes

<h1 id="errors"></h1>

## Errors

<table>
  <tr>
    <th>error</th>
    <th>description</th>
  </tr>
  <tr>
    <td><code>SyntaxError</code></td>
    <td>often the result of a typo, indicates syntax is incorrect</td>
  </tr>
  <tr>
    <td><code>ReferenceError</code></td>
    <td>indicates a variable does not exist (undefined or undeclared)</td>
  </tr>
  <tr>
    <td><code>URIERROR</code></td>
    <td>indicates special characters were not escaped when they needed to be</td>
  </tr>
  <tr>
    <td><code>TypeError</code></td>
    <td>results from an incorrect or unexpected data type</td>
  </tr>
  <tr>
    <td><code>Error</code></td>
    <td>generic object template from which other errors are created</td>
  </tr>
  <tr>
    <td><code>RangeError</code></td>
    <td>when a range is called with a number that doesn't exist within it, like a 4 being used on an array with length 2</td>
  </tr>
  <tr>
    <td><code>Nan</code></td>
    <td>not really an error, but indicates something is not a number, which can be unintended</td>
  </tr>
</table>

<h1 id="debugging"></h1>

## Debugging

The `console` object is useful for figuring out what is happening and where. The `log()` method will log to the browser console. Similarly, `info()` can be used to note in the console, `warn()` will indicate a warning, and `error()` will sign an error.

To create a noticeable block of logs, you can start a `console.group('group name here')` and fill it with logs and whatnot. To end the group, just call `console.groupEnd()`.

`console.table(<objectName>)` will display and object in a table format in the console.

`console.assert(<conditional>, <if condition is false, log what's here>)` allows logging only if something goes wrong.

[Return to table of contents](../README.md)
