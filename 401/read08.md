# SOLID
SOLID is known as first five object oriented design pronciples.

SOLID is stands for :
+ S - Single-responsiblity Principle
+ O - Open-closed Principle
+ L - Liskov Substitution Principle
+ I - Interface Segregation Principle
+ D - Dependency Inversion Principle

#### Single-Responsibility Principle:
SRP means that each class should only have one job, so if you end up creating a class which have alot pf jobs you should devide each job in a seperate class.

#### Open-Closed Principle:
OCP means that the Objects should be open for extension but should be close for modification, so the class should accept extending but refuse modifying.

#### Liskov Substitution Principle:
this principle means that every subclass should be substitutable for its parent class.

#### Interface Segregation Principle:
> A client should never be forced to implement an interface that it doesn’t use, or clients shouldn’t be forced to depend on methods they do not use.~quoted from https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design

#### Dependency Inversion Principle:
>Entities must depend on abstractions, not on concretions. It states that the high-level module must not depend on the low-level module, but they should depend on abstractions.~quoted from https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design

![solid](https://miro.medium.com/max/1400/1*XOMTPWTpDLypkp079p9XXg.png)


#### The SOLID Principles in Real Life
+ one of the benefits of using the SOLID principls in your code is that the code will be easier to maintain.

+ when using a single responsibility principle you dont have to worry about too much functionality in the class , you will concern only for one functionality so you wont be distracted by side errors.

+ in linskov substitution principle any child type of a parent type should be able to stand in for that parent without things blowing up. 

+ in interface segregation principle  you should favor many, smaller, client-specific interfaces over one larger, more monolithic interface. 

+ in dependency inversion principle its better to write code that depends upon abstractions rather than upon concrete details. 


## [BACK](../README.md)