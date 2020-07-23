<head>
  <style>
    code {
      color: green;
    }
  </style>
</head>

### Class 14 Reading Notes Part 1

<h1 id="transforms"></h1>

## CSS Transforms

The transform property allows manipulation of elements. It isn't supported by all browsers, so to use it, best practice would have you write it 4 times:

<pre>
<code style="color: green;">-webkit-transform: scale(1.5); /* for chrome */
-moz-transform: scale(1.5); /* for firefox */
-o-transform: scale(1.5); /* for opera */
transfor: scale(1.5); /* in case the browser just supports it */</code>
</pre>

Using transform, you can rotate an element by a value of degrees: `rotate(10deg);`. Or you can adjust an items scale where less than 1 is smaller and greater than 1 is larger: `scale(.75);`. Translate will move an element similarly to relative positioning: `translate(10px, 20%);`. Skew distorts elements along their x and y axis: `skew(10deg, 5deg);`.

<h1 id="transitions"></h1>

## CSS Transitions and Animations

Transitions can alter an element's appearance and behavior on a state change (like hover). Animations set multiple points of transition on different keyframes.

With transitions, you set things like timing of an element's transition by targeting the base element. And then you target the element again with a pseudo class defining the state change (like `:hover`) and tell it what to transition to.

Note that not all properties can be transitioned. 

[Return to table of contents](../README.md)
