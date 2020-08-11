### Class 02 Reading Notes

## JQuery

JQuery is a JavaScript library that makes DOM manipulation quick and clean. It allows a developer to access elements using CSS selectors. These elements are stored in JQuery objects, which are similar to DOM nodes.

```
// this would target the element with id="sandwiches"
$('#sandwiches')
```

Similar to DOM nodes, those JQuery objects and be used to manipulate the elements with methods:

```
// this would add the class "deli-food" to the element
$('#sandwiches').addClass('deli-food');
```

JQuery has a handy method to call on the document object that will wait for the page to load before triggering the code:

```
$(document).ready(function() {
  // do stuff
});
```

But this can be shortcut to just:

```
$(function() {
  // do stuff
})
```

When capturing a list of elements, you can iterate over them easily with the each() method and using 'this' to refer to each individual element in the list:

```
$('p').each(function() {
  let elID = this.id;
  $(this).addClass('paragraphs');
  console.log(`added paragraphs class to ${elID}`);
})
```

---

## Pair Programming

#### Six reasons to pair program:

1. It's more efficient. While it often does take longer, the code comes out cleaner and more bugs are caught in the process. This saves time on the back end and most importantly it helps prevent errors making it to release.
1. It keeps developers engaged. Having a partner keeps the process interesting and makes it less likely to end up distracted with something unrelated.
1. Pairing creates an opportunity to learn from peers. Everyone has different perspectives and techniques. Pair programming exposes developers to different styles where they would normally not advance out of their current skill set.
1. It improves social skills. And teams successes are directly related to their members social awareness.
1. Using shared screens is a very similar activity to white boarding for an interview. It requires practice describing and writing code and logic. So pair programming is great way to improve interviewing ability.
1. Pair programming is often a tool used by companies to onboard new employees. Already being comfortable and capable with the process helps new employees excel.

[Return to table of contents](../README.md)

