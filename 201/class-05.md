<head>
  <style>
    code {
      color: green;
    }
  </style>
</head>

### Class 05 Reading Notes

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

Interesting note about image placement: `<img>` is an inline element. So if you place it inside a block level element like `<p>`, it will sit inside the text