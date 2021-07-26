# Primitives vs. Objects

## there are two main types in java system:
1. ## primitives : int , boolean ..etc . 
2. ## reference : Integer , Boolean ..etc .

## 1. primitives:
+ ## Every primitive type corresponds to a reference type.

## primitice variables size on memory :
+ ## boolean – 1 bit
+ ## byte – 8 bits
+ ## short, char – 16 bits
+ ## int, float – 32 bits
+ ## long, double – 64 bits

## these values can vary depending on virtual machine implementation , also they live in the stack and they are accessed very fast.

## 2. reference :
+ ## reference types are objects, and they live on the heap so they are slow to access in relative to primitives.

## single instant of reference size in memory:
+ ## Boolean – 128 bits
+ ## Byte – 128 bits
+ ## Short, Character – 128 bits
+ ## Integer, Float – 128 bits
+ ## Long, Double – 192 bits

## Performance
## java performance depends on the hardware on which the code runs, on the compiler, on the state of virtual machine, and on other proccesses activity in the system.

## java default values:

| type                   | default value                          |
| -----------            | -----------                            |
| numeric types          | 0                                      |
| boolean                | false                                  |
| char                   | \u0000                                 |
| wrapper classes        | null                                   |

# Exception

> ## An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions.~quoted from https://docs.oracle.com/javase/tutorial/essential/exceptions/definition.html

## there is an object called exception object, which created when an error occurs whithin a method, this object contains information about the error, including its type and the state of the programwhen the error occured.

## the code which might throw exceptions must be enclosed by one of these:
1. ## A try statement that catches the exception. 
2. ## A method that specifies that it can throw the exception.

> ## All methods use the throw statement to throw an exception. The throw statement requires a single argument: a throwable object. Throwable objects are instances of any subclass of the Throwable class. 
## Here's an example of a throw statement.

```
public Object pop() {
    Object obj;

    if (size == 0) {
        throw new EmptyStackException();
    }

    obj = objectAt(size - 1);
    setObjectAt(size - 1, null);
    size--;
    return obj;
}
```

## throwable classes :
![throwable](https://docs.oracle.com/javase/tutorial/figures/essential/exceptions-throwable.gif)


# Scanning
## we use scanning to break down formatted input into tokensand translate individual tokens according to their type.

## example about scanner:

```
import java.io.*;
import java.util.Scanner;

public class ScanXan {
    public static void main(String[] args) throws IOException {

        Scanner s = null;

        try {
            s = new Scanner(new BufferedReader(new FileReader("xanadu.txt")));

            while (s.hasNext()) {
                System.out.println(s.next());
            }
        } finally {
            if (s != null) {
                s.close();
            }
        }
    }
}
```

## [BACK](../README.md)