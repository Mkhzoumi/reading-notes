# Packages and Import

+ ## in java, packages means directory, so when we say package name its just the same as directory name which contains the .java files .
+ ## we declare packages when we define our java program .
+ ## if you want to use packages from other libraries you have to name the packages in an import statement .

## Package declaration
+ ## in your code after the optional package declaration, you can have an import statement to specify classes from other packages .

## Statement order in the java file is as the following:
1. ## Package statment (optional).
2. ## Imports (optional).
3. ## Class or interface definitions.

## Imports options:
1. ## make all the classes from the imported file visible.

```
import javax.swing.*;  // Make all classes visible altho only one is used.

class ImportTest {
    public static void main(String[] args) {
        JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```

1. ## make a single class visible from the imported file.

```
import javax.swing.JOptionPane;  // Make a single class visible.

class ImportTest {
    public static void main(String[] args) {
        JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```

1. ## we can use classes from another file by fully qualified class name without import.

```
class ImportTest {
    public static void main(String[] args) {
        javax.swing.JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```

## most common imports

+ ## import java.awt.*;	Common GUI elements.
+ ## import java.awt.event.*;	The most common GUI event listeners.
+ ## import javax.swing.*;	More common GUI elements. Note "javax".
+ ## import java.util.*;	Data structures (Collections), time, Scanner, etc classes.
+ ## import java.io.*;	Input-output classes.
+ ## import java.text.*;	Some formatting classes.
+ ## import java.util.regex.*;	Regular expression classes.


## some facts about importing in java
+ ## import wont make the file larger because the import is only tell the compiler where to look.
+ ## there are no different if we imported all classes or imported only one class .


# Loops
> ## In programming languages, looping is a feature which facilitates the execution of a set of instructions until the controlling Boolean-expression evaluates to false.~quoted from https://www.baeldung.com/java-loops

## types of loops in Java:
+ ## for loop: allows us to repeat certain operations by incrementing and evaluating a loop counter.
+ ## for-each loop
+ ## While loop: repeats a statement or a block of statements while its controlling Boolean-expression is true.
+ ## Do-While loop: works like the while loop but it excute the code at least once.


## [BACK](../README.md)
