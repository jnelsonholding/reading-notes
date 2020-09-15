### Class 02 Reading Notes

## Java Imports

In Java, a lot of broader functionality has been added in the form of classes and methods. But to make use of that pre-built code, you have to tell Java what you need. Importing is the cleanest way to communicate that. Here's an example of the format for importing the LocalDateTime type:

```
import java.time.LocalDateTime;

public class Sample {
  public static void main(String[] args) {
    LocalDateTime now = LocalDateTime.now();
    ...
  }
}
```

It is possible to just access the classes in line (for example: `java.time.LocalDateTime.now()`). But this can cause a lot of repetitive writing and looks a lot less clean. Plus most IDE's can recognize if you are using a class and will auto-create the import line where possible.

## Java Loops

There are 3 basic types of loops in Java: For loop, While loop, and Do-While loop. Here are some examples of their available formats:

- For loops
  - Simple:
  ```
  for (int i = 0; i < arr.length; i++) {
    System.out.println(arr[i]);
  }
  ```
  - Labeled: (good for break statements in nested loops)
  ```
  aa: for (int i = 0; i < arr.length; i++) {
      System.out.println(arr[i]);
      bb: for (int j = 0; j < 3; j++) {
        if (arr[i] == j) {
          break aa;
        }
      }
    }
  ```
  - Enhanced: (shorthand to access elements in arrays or collections)
  ```
  for (int val : intArr) {
    System.out.println(val);
  }
  ```
  - forEach:
  ```
  stringArr.forEach(str -> System.out.println(str));
  ```
- While Loops
  ```
  while (bigSpiderIsInTub) {
    System.out.println("AHHHH");
    if (attemptRemoveSpider() == "success") {
      bigSpiderIsInTub = false;
    }
  }
  ```
- Do-While Loops
  ```
  do {
    System.out.println("This only runs once");
  } while (false);
  ```

[Return to table of contents](../README.md)
