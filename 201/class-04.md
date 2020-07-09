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











































