# Objects and Classes

## objects are everything which have a state and behavior.
### benefits of bundling the code into individual objects:
+ ### Modularity: The source code for an object can be written and maintained independently.
+ ### Information-hiding: the details of its internal implementation remain hidden from the outside world.
+ ### Pluggability and debugging ease: If a particular object turns out to be problematic, you can simply remove it from your application and plug in a different object as its replacement.


## classes are the blueprint or template which make the objects.
## class example:

```
public class Bicycle {
        
    // the Bicycle class has
    // three fields
    public int cadence;
    public int gear;
    public int speed;
        
    // the Bicycle class has
    // one constructor
    public Bicycle(int startCadence, int startSpeed, int startGear) {
        gear = startGear;
        cadence = startCadence;
        speed = startSpeed;
    }
        
    // the Bicycle class has
    // four methods
    public void setCadence(int newValue) {
        cadence = newValue;
    }
        
    public void setGear(int newValue) {
        gear = newValue;
    }
        
    public void applyBrake(int decrement) {
        speed -= decrement;
    }
        
    public void speedUp(int increment) {
        speed += increment;
    }
        
}
```

> ##This is a class declaration. The class body (the area between the braces) contains all the code that provides for the life cycle of the objects created from the class: constructors for initializing new objects, declarations for the fields that provide the state of the class and its objects, and methods to implement the behavior of the class and its objects.

```
class MyClass {
    // field, constructor, and 
    // method declarations
}
```

## class declarations can include these components:
+ ### Modifiers such as public, private, and a number of others that you will encounter later.
+ ### The class name .
+ ### The name of the class's parent (superclass), if any, preceded by the keyword extends.
+ ### A comma-separated list of interfaces implemented by the class, if any, preceded by the keyword implements.
+ ### The class body, surrounded by braces {}.

## variables are three kinds:
+ ### Member variables in a class—these are called fields.
+ ### Variables in a method or block of code—these are called local variables.
+ ### Variables in method declarations—these are called parameters.

## modifiers types:
+ ### public modifier—the field is accessible from all classes.
+ ### private modifier—the field is accessible only within its own class.

## methods declaration components:
1. ### Modifiers—such as public, private, and others you will learn about later.
2. ### The return type—the data type of the value returned by the method, or void if the method does not return a value.
3. ### The method name—the rules for field names apply to method names as well, but the convention is a little different.
4. ### The parameter list in parenthesis—a comma-delimited list of input parameters, preceded by their data types, enclosed by parentheses, (). If there are no parameters, you must use empty parentheses.
5. ### An exception list—to be discussed later.
6. ### The method body, enclosed between braces—the method's code, including the declaration of local variables, goes here.

## when it comes to naming a method we use the cammel case rule, and in the same class you can give methods the same name as long as they have different parameter list.

# Decimals
> ## Every digit in a decimal number has a "position", and the decimal point helps us to know which position is which:

![decimal](https://www.mathsisfun.com/numbers/images/decimal.svg)

+ ## Every position further to the left is 10 times bigger, and every position further to the right is 10 times smaller.

+ ## decimal number system it also called big10 system , because it based on number 10.


## there are other types of number systems like binary, and there is hexadecimal:

+ ### Binary Numbers: binary numbers are based on 2 numbers 0 , 1.
+ ### Hexadecimal Numbers:They look the same as the decimal numbers up to 9, but then there are the letters ("A',"B","C","D","E","F") in place of the decimal numbers 10 to 15. 


## [BACK](../README.md)