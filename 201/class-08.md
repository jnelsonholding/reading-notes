<head>
  <style>
    code {
      color: green;
    }
  </style>
</head>

### Class 08 Reading Notes

<h1 id="cssfloats"></h1>

## CSS Floats

For the first part of CSS Layout, go [here](class-04.md#csslayout)

We've already looked at floats briefly. To recap, they cause an element to "float" left or right as far as it can in its container. Other elements in normal flow will actually flow around the floated element.

For instance, floating a block element right would allow a paragraph underneath it to flow up left next to the block element.

`float: left;` is commonly used as a convenient way to place elements next to each other. This can be tricky because boxes with different heights can sort of catch each other in positions that make them display out of order. But there is a way to deal with that.

The `clear` property can be used to keep a box's sides "clear" of touching other boxes. How this can be used with `float: left;`, for example, is to `clear: left;` a box that could catch on another one. This will make the box not accept sitting with another element touching its left side. And it will move down until it's allowed to slide to the left of its container. The next elements in line should then fall in line after it.

`clear` can also specify `right` to keep its right side clear. The value `both` keeps both left and right clear. And `none` allows the element to once again touch on both sides.

Parent elements of floated elements can have issues. In some browsers, they will become 0px tall, creating essentially an empty line. There are two properties to set for the parent element to deal with this issue: `overflow: auto;` and `width: 100%;`. This will cause the containing element to expand to the size of its floated child element.

<h1 id="cssdesign"></h1>

## CSS Layout Design

Floating containers left is a method to create columns. Just by setting the width of two containers to equal to less than the screen width, the second container will float up to the right of the first container, creating columns.

A common width for designers to focus on for screen size is 1000px. It will display well enough on most screens. The top 600px are often all a user will see without scrolling. So that 1000px by 600px area is the most important to convince the user that they should explore further.

A couple options for layout design are fixed width and liquid. Fixed width would have box widths hard coded using px, which allows for a lot of control but can be a challenge with screen sizes. Liquid layouts have widths set with percentages allowing them to stretch. But they are difficult to control with that much flexibility.

Working in a grid can help design control and continuity throughout a website. Many designers opt for a 960px wide grid with 12 60px columns (each with a margine of 10px).

A framework for a 960 grid is available at https://960.gs/.

An alternative to linking multiple stylesheets in the head of your HTML is importing them into one CSS file. Placing `@import url("reset.css")` in the first line of your main styles.css file would run the reset first before running the styles.css code.

[Return to table of contents](../README.md)

























