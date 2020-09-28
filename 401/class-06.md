### Class 06 Reading Notes

## Inheritance

In Java, a class can inherit state and behavior from another class. In this relationship, the class that is inherited from is call a *super class* and the class that inherits is a *subclass*. A class can only ever inherit from one super class. Conversely, a class can have unlimited subclasses.

## Interface

An interface is a template of empty methods that can be *implemented* by a class. Interfaces can be implemented by multiple classes. But since the methods in the interface are empty, they only act as formalized requirement for a method to exist in a class. The class itself will need to define the method according to its own needs.

A major difference between class inheritance and using implementing interfaces is that interfaces do not have fields. So interfaces are used to formalize behavior but not state.

## Package

A package is essentially a folder for Java files/classes. Because Java libraries can become extensive, packages provide organization within a library for separating the many classes created.

## Object Class

Every class is a subclass in the Object class' eyes. It provides some methods that offer generic functionality. Most of them can be overwritten in the subclasses. Here are some of the methods.

  - clone() : creates a copy of an object, requires the Cloneable interface be implemented
  - equals() : tests if the object passed is exactly the same object, can be overwritten to check for equivalency instead, but consider writing that test into a new method
  - finalize() : may be called when an object is up for garbage collection, but not always, must be overwritten to do anything, but is also not very reliable
  - getClass() : returns class name, can't be overwritten
  - hashCode() : returns the object's memory address in hexadecimal, should be overwritten when equals() is changed because it is intrinsically tied to the equality of objects
  - toString() : returns a string representation of an object, should be overwritten to make objects human readable

[Return to table of contents](../README.md)
