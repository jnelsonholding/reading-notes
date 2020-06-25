### Notes on JavaScript

JavaScript can be simplified into 4 major actions:

- Access - accessing content of the page
- Modify - modifying the content
- Program - defining rules or instructions for the browser
- React - reacts to events triggered by the user or the browser

#### Writing a script

A script is used to complete a goal (output or result). So to write one, it's important to define the goal first. Follow these steps:

- Define the goal of the script.
- Design the script by considering the inputs available and splitting the steps required to reach the goal into smaller goals. Each step can be represented in a flowchart.
- Take the map created and code each portion of it. Once each individual goal is met in succession, the end goal of the script should also be complete.

#### Operators

Arithmetic:
name | symbol | description
:--- | :---: | :---
Addition  | + | adds two values
Subtraction | - | subtracts a value from another
Division | / | divides a value from another
Multiplication | * | multiplies two values
Increment | ++ | adds 1 to a value
Decrement | -- | subtracts 1 from a value
Modulus | % | returns the remainder after dividing a value from another

String:
name | symbol | description
:---|:---:|:---
Concatenate | + | glues two strings together

I'm sure there are more string operators. Would be worth looking up.

#### Functions

Functions can be called to run repeatable blocks of code. Much like `var` for a variable, a function is declared using its keyword followed by its name:
```
function functionName() {
    code block goes here;
}
```

A function also allows for parameters, which are like personal variables for the function to use when it runs.
```
function functionName(parameter1, parameter2) {
    code block goes here;
}
```

When calling a function, the values use for the parameters are called arguments.
```
functionName(parameter1 = argument1, parameter2 = argument2)
```

When you want a function to output a value, use `return`. In the following function, the value of `c` would be output:
```
funSum(a, b) {
    c = a + b;
    return c;
}
```

[Return to table of contents](README.md)