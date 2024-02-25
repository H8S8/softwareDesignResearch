# Software Design Reseach

## Principle Design Strategies

### 1. Structured Design
Structured design, otherwise known as modular design, breaks a program down to many smaller parts (solution modules). These solution modules are carefully arranged to provide a solution to the main problem. This improves the reusability of the code and through abstraction, its readability. This is an example of top-down design.

### 2. Function Oriented Design
In Function Oriented design, the program is broken down into a set of sub-systems (functions), where each has a unique defined purpose. Like Structured Design, this is also an example of top-down design. When a function is called, the state of the program changes. Functional Design is best used when the program relies on inputs as opposed to the state of the program.

### 3. Object Oriented Design
Object Oriented design (Object Oriented Programming - OOP) is based around different entities and their characteristics.


## Answers to Questions

### 1. What do we mean by coupling and cohesion when discussing structured design?
Coupling describes how much the different modules depend on eachother. I.e. a high degree of coupling would indicate that changes in one module would likely affect other modules. Cohesion quantifies how well the elements within a particular module work together to achieve a single goal. I.e. low cohesion would indicate that the different elements in the module are not closely related and serve several purposes. Good structured design has high cohesion and low coupling.

### 2. What is the difference between top-down and bottom-up design? Which best describes a function oriented design?

In top-down design, a process is broken down into several sub-processes. These sub-processes could then be further decomposed until the most basic level of functionality in this hierarchy is reached. This approach is useful when you are designing a bespoke piece of software from scratch.</br>
Bottom-up design, however, begins with the creation of the most basic components. More complex entities can then be created using the basic components. This approach is useful when you are working with a pre-existing system where these basic initial components are avaliable.</br>
Bottom-up design best describes OOP as through inheritance and interfaces it makes use of basic building blocks (abstract classes) to create more complex classes. 

### 3. In which design methodology would a class diagram be most useful?
A class diagram would be most useful in OOP as this is the only type of design that makes use of complex relationships between different classes.

### 4. What are the four pillars of object oriented programming? Give a single-sentence description of each.
- <b>Abstraction:</b> the functionality of an abstract method/ object is clear, but the exact implmentation of it is hidden.
- <b>Encapsulation:</b> limiting access to certain parts of your code.
- <b>Inheritance:</b> one object can aquire the proporties and methods of a parent object.
- <b>Polymorphism:</b> objects of different classes which share an inheritance chain can be used interchangably.

### 5. What is the strategy pattern? How would its implementation differ between a functional and object oriented system?
A strategy pattern is a type of software design that allows the method of implementation to be chosen at runtime.</br>
In function oriented design, a function is chosen from a set of possible functions.</br>
In OOP, you could create an interface which is implemented by the different interchangable strategies.

### 6. Imagine your is creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.

I would suggest OOP. Different items could be dynamically added to the system through the use of Polymorphism. A 'PurchasableItem' interface could be implemented for anything, from a takeaway to a new coat. The bottom-up design of OOP allows you to create the basic building blocks for a system from which higher level entities can be created. The basic system can be modified to work across any sector.

## Resources List

https://www.tutorialspoint.com/software_engineering/software_design_strategies.htm
https://www.sciencedirect.com/topics/computer-science/structured-design
https://www.geeksforgeeks.org/software-engineering-coupling-and-cohesion/
https://www.freecodecamp.org/news/four-pillars-of-object-oriented-programming/
https://www.geeksforgeeks.org/structured-analysis-and-structured-design-sa-sd/
https://www.geeksforgeeks.org/software-engineering-function-oriented-design/
https://en.wikipedia.org/wiki/Strategy_pattern
