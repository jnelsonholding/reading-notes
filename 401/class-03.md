### Class 03 Reading Notes

## Primitives vs Objects

In Java, you can use primitives directly or you can use wrapper objects. The difference is subtle:

```
// regular assignment of an int primitive
int i = 1;

// called 'autoboxing', converts the primitive into its object wrapper
Integer j = 1;

// called 'unboxing', uses the wrapped object as a reference to assign a primitive
int k = new Integer(1);
```

The basic use of a primitive assignment in the first example is usually more space efficient. Storing a value in its object wrapper can in some cases use much more space, depending on the type.

Are there advantages to using the object wrapper for these primitive data types? I haven't seen one yet. If you know of one, let me know!

[Return to table of contents](../README.md)
