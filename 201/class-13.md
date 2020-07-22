<head>
  <style>
    code {
      color: green;
    }
  </style>
</head>

### Class 13 Reading Notes

<h1 id="localstorage"></h1>

## Local Storage

Storage has been an issue for web development since its beginnings. It's necessary because in certain situations, constant retrieval of data from a server can cause major slowdowns for the user. So ideally, you would keep as much local as possible.

HTML5 has 'Web Storage', also known as 'local storage' and 'DOM storage'. It provides a way to store key-value pairs client side. This is accessed through the object `localStorage'. For instance, to set a key-value pair, you would do this:

`localStorage.setItem('savedInt', 5);`

What's awesome about this is you can do it right now. Just open up your console and type that. If you refresh the page, it'll still be saved! You can then get your value by calling the key:

`// returns 5`  
`localStorage.getItem('savedInt');`

Did you know that you can probably run a local SQL database as well? Seriously what? Well keep in mind you can only use 5 MB, so don't go crazy with it.

[Return to table of contents](../README.md)
