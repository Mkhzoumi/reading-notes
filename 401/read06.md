# Object-Oriented Programming Concepts

## Inheritance
+ when a different objects have share some common characteristics, object oriented programming allows classes to inherit commonly used state and behavior from other classes.
+ Important thing to know that in java programming laguage, each class is allowed to have one one direct superclass, and each superclass is allowed to have unlimited number of subclasses. 
+ subclass: A class that is derived from another class, also known as (derived class, extended class, or child class).
+ superclass: The class from which the subclass is derived, also known as (base class or a parent class).
+ Classes can be derived from classes that are derived from classes that are derived from classes, and so on.
+ A subclass does not inherit the private members of its parent class. However, if the superclass has public or protected methods for accessing its private fields, these can also be used by the subclass.


![inheritance](https://it-solutions.center/wp-content/uploads/2020/03/java-inheritance-introduction.png)

### The syntax for creating a subclass:

```
class MountainBike extends Bicycle {

    // new fields and methods defining 
    // a mountain bike would go here

}
```

# Interface
+An interface is a group of related methods with empty bodies.
+ In java an interface is: a reference type, similar to a class, that can contain only constants, method signatures, default methods, static methods, and nested types. 
+  Interfaces cannot be instantiated—they can only be implemented by classes or extended by other interfaces.

example:

```
interface Bicycle {

    //  wheel revolutions per minute
    void changeCadence(int newValue);

    void changeGear(int newValue);

    void speedUp(int increment);

    void applyBrakes(int decrement);
}
```

> Implementing an interface allows a class to become more formal about the behavior it promises to provide. Interfaces form a contract between the class and the outside world, and this contract is enforced at build time by the compiler. If your class claims to implement an interface, all methods defined by that interface must appear in its source code before the class will successfully compile. ~quoted from https://docs.oracle.com/javase/tutorial/java/concepts/interface.html

![interface](https://techvidvan.com/tutorials/wp-content/uploads/sites/2/2020/02/difference-between-class-and-interface-in-java.jpg)


# Package
+ A package is a namespace that organizes a set of related classes and interfaces.
+ The Java platform provides an enormous class library (a set of packages) suitable for use in your own applications. This library is known as the "Application Programming Interface", or "API" for short. 

## [BACK](../README.md)