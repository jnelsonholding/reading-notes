### JS Operators and Loops

Comparison operators:

symbol | operation
:---: | ---
== | is loosely equal to
=== | is strictly equal to
!= | is loosely not equal to
!== | is strictly not equal to
> | is greater than
< | is less than
>= | is greater than or equal to
<= | is less than or equal to

Logical operators:

symbol | operation
:---: | ---
a && b| returns true if a and b are both true
a &#124;&#124; b | returns true if either a or b are true
!(a) | returns true if a is false - not(this)

While loops:

A while loop will repeatedly execute its code block while its condition evaluates to true:

```
while (this is true) {
    do this code block repeatedly until that becomes false
}
```

Once the conditional (this is true) statement becomes false, the code block will be bypassed and the JS moves onto whatever follows the while loop section.

For loops:

A for loop repeats its code block for as many repetitions as are specified by its condition. Essentially, it is a while loop where the conditional counts down how many times it's run to decide when it is false and will move on.

```
for (var i = 0, i < 10, i++) {
    do this code block
}
```

That code could be read as: for a variable i that starts at 0 and increases by 1 for every code block run, while i is less than 10, run the code block.

That sounds like gibberish, but it boils down to "run this code 10 times then move on."

[Return to table of contents](README.md)