# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.
> 

Prototype Pattern:

Prototype Pattern solves the problem of creation of object when it is time consuming or redundant. It helps to copy an existing object instead of creating new instance from scratch.

Basic Idea:
The pattern works by creating clones using a clone method. It lets us create copies of objects without depending on the concrete classes.

Advantages and Disadvantages:
We can clone objects without tightly coupled to concrete class
Cloning objects that might have circular references is difficult

Summary: 
A prototype interface declares the method for cloning. Then the concrete prototype class implements the cloning method. The client class can produce of copy of any object that follows the prototype interface.

Decorator Pattern:

Decorator Pattern solves the problem of adding new functionality and behavior to an object without affecting the behavior of other existing objects within the same class

Basic Idea:
It works by creating a decorator class which wraps the original class and provided additional functionality keeping class methods signature intact.

Advantages and Disadvantages:
We can extend an object's behavior without making new subclass. Code maintainability will be difficult when many similar decorators are created.

Summary:
First an interface has to be created. Then concrete class implements this interface. An abstract decorator class implements the interface. The concrete decorator class extends the abstract decorator class, to decorate interface objects.

Observer Pattern:

Observer pattern is used when any change in objects state has to notified to subscriber object. It is like the our internet banking notification that notifies us both to our mobiles and emails or live match updates when the score changes.

Basic Idea:
When there is 1:n relationship between objects such as if one object is modified, the dependent objects can be notified automatically

Summary:
It uses Subject, Observer and Client class. Subject class has methods to attach and detach observers from the client. An abstract class observer and concrete class subject that extends observer class

Advantages and Disadvantages:
Loosely coupling among objects that interact with each other. Observers can be removed at any point of time

Adapter Pattern:

It solves the problem of making two incompatible interfaces interact with each other. one such example is our power plugs that varies across various countries

Basic Idea:
It basically implements a class that bridges the gap betwwen expected interface and existing class and helps us avoid any changes to existing code and associated side-effects

Advantages and Disadvantages:
Advantage of adapter pattern is that we don't need to change the existing class or interface. Disadvantage is complexity of code increases as new class/interfaces are introduced.

Summary:
Adaptor pattern introduces a adapter class between interface and existing class. The adapter class implements the expected interface and keeps a reference to an object we want to reuse. The methods defined by the interface call a method on referenced object and return a value of expected type. This way the class fulfils the expected idea by implementing interface and enables us to reuse existing incompatible implementations









