# Java Basics

## Variables

| Variable kind                          | description                                               |
| -----------                            | -----------                                               |
| Instance Variables (Non-Static Fields) | their values are unique to each instance of a class       |
| Class Variables (Static Fields)        | any field declared with the static modifier               |
| Local Variables                        | only visible to the methods in which they are declared    |
| Parameters                             | variables passed as arguments to methods                  |

## Naming a variable

## in java there are some rules you have to follow when it comes to naming a variable:

+ ## Variables names are case sensitive
+ ## Must start with a letter
+ ## Full words is much better than cryptic abbreviations
+ ## If it consists of more than one word, capitalize the first letter of each subsequent word


## Operators

## operators of java programming language:

| Operator               | Sympol                                   |
| -----------            | -----------                              |
| postfix                | expr++ expr--                            |
| multiplicative         | * / %                                    |
| additive               | + -                                      |
| shift                  | << >> >>>                                |
| relational             | < > <= >= instanceof                     |
| equality               | == !=                                    |
| bitwise AND            | &                                        |
| bitwise exclusive OR   | ^                                        |
| bitwise inclusive OR   | \|                                       |
| logical AND            | &&                                       |
| logical OR             | \| \|                                    |
| ternary                |  ? :                                     |
| assignment             | = += -= *= /= %= &= ^= \|= <<= >>= >>>=  |

## Expressions, Statements, and Blocks

## expressions are made up of variables, operators, and method invocations , for example:-

```
int cadence = 0;
anArray[0] = 100;
System.out.println("Element 1 at index 0: " + anArray[0]);

int result = 1 + 2; // result is now 3
if (value1 == value2) 
    System.out.println("value1 == value2");
```

## Statements
## A statement forms a complete unit of execution.

## statement types:
+ ## Assignment expressions
+ ## Any use of ++ or --
+ ## Method invocations
+ ## Object creation expressions

## expression statement example:-

```
// assignment statement
aValue = 8933.234;
// increment statement
aValue++;
// method invocation statement
System.out.println("Hello World!");
// object creation statement
Bicycle myBike = new Bicycle();
```

## declaration statements example:-

```
// declaration statement
double aValue = 8933.234;
```

## Blocks
## A block is a group of statements between braces, can be used anywhere a single statement is allowed.

## block example:-

```
class BlockDemo {
     public static void main(String[] args) {
          boolean condition = true;
          if (condition) { // begin block 1
               System.out.println("Condition is true.");
          } // end block one
          else { // begin block 2
               System.out.println("Condition is false.");
          } // end block 2
     }
}
```

## Control Flow Statements

> ### flow statement break up the flow of execution by employing decision making, looping, and branching, enabling your program to conditionally execute particular blocks of code. ~ quoted from https://docs.oracle.com/javase/tutorial/java/nutsandbolts/flow.html

## compile code

> ### When you compile code, the compilor (usually another program) takes the program the human wrote, and converts it into the program the computer can understand (i.e. converts from Java to machine language). The very short version could be, yes, compile means to make the code executable. ~ quoted from https://www.reddit.com/r/explainlikeimfive/comments/233dq5/eli5_what_does_it_mean_to_compile_code/




# [back](../README.md)