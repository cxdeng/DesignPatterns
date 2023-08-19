# Design Patterns

# 1. Overview of Design Patterns

## 1.1 The background of software design pattern


The concept of "design patterns" did not originally appear in software design, but was used in the design of architecture. In 1977, the renowned American architect and the director of the Center for Environmental Structure at the University of California, Berkeley, Christopher Alexander, described some common architectural design problems in his book "A Pattern Language: Towns, Buildings, Construction." He introduced 253 basic patterns for designing towns, neighborhoods, residences, gardens, and rooms.

By 1990, the software engineering community began discussing the topic of design patterns and subsequently held several conferences on the subject. It wasn't until 1995 that Erich Gamma, Richard Helm, Ralph Johnson, and John Vlissides co-authored the book "Design Patterns: Elements of Reusable Object-Oriented Software." This book included 23 design patterns, marking a milestone in the field and leading to a breakthrough in software design patterns. These four authors are also famously known in the software development domain as the "Gang of Four" or GoF.



## 1.2 The concept of software design patterns

A Software Design Pattern, also simply known as a Design Pattern, is a collection of code design experiences that are repeatedly used, widely known, categorized, and summarized. It outlines the recurring problems faced during the software design process and their respective solutions. That is to say, it embodies a series of approaches to address specific issues, capturing the accumulated design wisdom of past practitioners. These patterns hold general applicability and can be used over and over again.



## 1.3 The necessity of learning design patterns.

The essence of design patterns is the practical application of object-oriented design principles, reflecting a deep understanding of class encapsulation, inheritance, polymorphism, as well as the relationships and compositions among classes.

**Proper use of design patterns has the following advantages:**

1. It enhances the thinking, programming, and design capabilities of programmers.
2. It standardizes program design and makes code development more systematic, greatly improving software development efficiency and thereby shortening the software development cycle.
3. It ensures that the designed code has high reusability, readability, reliability, flexibility, and maintainability.



## 1.4 Classification of Design Patterns

* **Creational patterns**

  Used for delineating "how objects are created," the primary feature is "decoupling the process of object creation from its utilization." The GoF (Gang of Four) book presents five creational patterns: Singleton, Prototype, Factory Method, Abstract Factory, and Builder.

* **Structural patterns**

  Used to outline how to organize classes or objects into larger configurations following certain structures, the GoF (Gang of Four) book introduces seven structural patterns: Proxy, Adapter, Bridge, Decorator, Facade, Flyweight, and Composite.

* **Behavioral Patterns**

  These are concerned with how classes or objects interact and collaborate to achieve tasks that an individual object can't undertake by itself, as well as how roles and duties are allocated. In the GoF (Gang of Four) book, eleven behavioral patterns are presented: Template Method, Strategy, Command, Chain of Responsibility, State, Observer, Mediator, Iterator, Visitor, Memento, and Interpreter.



# 2. UML Diagram

The Unified Modeling Language (UML) is a visual modeling language employed for software design. Its hallmarks include being straightforward, unified, graphical, and capable of conveying both dynamic and static aspects of software design.

UML approaches the target system from different angles and stipulates nine diagram types: use case diagrams, class diagrams, object diagrams, state diagrams, activity diagrams, sequence diagrams, collaboration diagrams, component diagrams, and deployment diagrams.



## 2.1 Class Diagram Overview

The Class diagram illustrates the static structure of a model, particularly the classes within the model, their internal makeup, and their interrelationships with other classes. Temporary information is not shown in class diagrams. They are an essential aspect of object-oriented modeling.



## 2.2 The role of class diagrams

* In software engineering, a class diagram is a static structural diagram that depicts a collection of classes within a system, along with their attributes and relationships. It serves to simplify people's comprehension of the system.
* A class diagram is a vital artifact of the system analysis and design phases, serving as a crucial model for system coding and testing.



## 2.3 Representation of a class diagram

### 2.3.1 Representation of a class diagram

In UML class diagrams, classes are represented by rectangles containing class names, attributes (fields) and methods (methods) with dividing lines, such as
The figure below shows an Employee class, which contains three attributes of name, age and address, and the work() method.

![](./img/Employee.jpg)

The plus and minus signs added before attribute/method names indicate the visibility of these attributes/methods. In UML class diagrams, there are three symbols used to represent visibility:

1. **Public (+):** Attributes or methods marked with a plus sign (+) are indicative of public visibility. They are accessible from any part of the system, including external classes and components.
2. **Private (-):** Attributes or methods marked with a minus sign (-) denote private visibility. They can only be accessed within the class where they are defined. They are not directly accessible from outside the class.
3. **Protected (#):** Attributes or methods marked with a hash sign (#) represent protected visibility. They can be accessed within the class where they are defined and by its subclasses. They are typically used in scenarios involving inheritance.

These symbols depicting visibility help define the scope and access permissions of attributes and methods in UML class diagrams, contributing to a comprehensive understanding of the class structure and interactions within a software system.

The full representation of the property is: visibility name :type [ = default value ]

The full representation of a method is: visibility name(parameter-list)[:return-type]

> Notice:
>
> 1. Items in square brackets are optional
> 2. There is also the type before the variable name, and the return value type before the method name



**Example:**

![](./img/demo.png)

The above figure shows that the Demo class defines three methods:

* **method() :** The modifier is public, there are no parameters, and there is no return value.
* **method1() :** The modifier is private, there are no parameters, and the return value type is String.
* **method2() :** The modifier is protected, it receives two parameters, the first parameter type is int, the second parameter type is String, and the return value type is int.