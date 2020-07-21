<head>
  <style>
    code {
      color: green;
    }
  </style>
</head>

### Class 12 Reading Notes

<h1 id="chartjs"></h1>

## Chart.js

Chart.js is a great way to display visual data on a page. It targets a `<canvas>` element and can create basic visual graphs with styling. Also, it can animate. Pretty handy. Here is a link to the docs:

[Chart.js Docs](https://www.chartjs.org/docs/latest/)

It looks like it's fairly easy to use and seriously versatile. I mean, [look at this bar graph](https://www.chartjs.org/docs/latest/charts/bar.html), that's so pretty.

Probably the best way to get it is using NPM. But it's also an option to download it and "build" it.

<h1 id="canvas"></h1>

## HTML Canvas

The `<canvas>` element is a container for rendering visuals. It's useful to give it an `id` attribute so it's easily targetable with JS. Also, it should have a specific width and height, which is fine to define directly in the HTML. Resizing with CSS runs the risk of distorting the image because it might not handle aspect ratio well.

An interesting feature of `<canvas>` is that you can specify fallback content between its opening and closing tags. Newer browsers will not display what is in between them, but an older browser that fails to handle the `<canvas>` tag will use what's inside. So this is totally above board:

`<canvas id="aGraph" width="300px" height="300px"><img src="puppy.jpg"></canvas>`

If the browser does not handle the `<canvas>` tag, then it will just disply puppy.jpg. Which can also be used for accessibility. For instance, if a user can't view the canvas, they can access the text between the tags.

There's a plethora of features available for drawing and styling. The docs have it all!

[Canvas API Docs](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)

[Return to table of contents](../README.md)
