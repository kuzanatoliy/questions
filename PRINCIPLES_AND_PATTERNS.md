# Principles and patterns

## SOLID

<details>
  <summary>What do you know about SOLID?</summary>

  In progress ...

</details>

## KISS

<details>
  <summary>What is KISS?</summary>

  KISS or keep it simple stupid is one of the design principles. KISS says that the many systems will work better if they are simple. So, simplicity should be one of the main targets in the design sphere.

</details>

## DRY

<details>
  <summary>What is DRY?</summary>

  DRY or don’t repeat yourself is one of the design principles. DRY says that not need to repeat different information or functionality. Each part of knowledge should have only one view into system scope.

</details>

## YAGNI

<details>
  <summary>What is YAGNI?</summary>

  YAGNI or you aren’t gonna need it is one of the design principles. YAGNI says that the programmer should not implement functionality if it is not necessary. There are a few reasons. Firstly, a customer does not have to pay for something that is not needed for him. Secondary, additional functionality could increase the development difficulty of other features.

</details>

## Design patterns

### Links
[What’s a design pattern?](https://refactoring.guru/design-patterns/what-is-pattern)
[Why should I learn patterns?](https://refactoring.guru/design-patterns/why-learn-patterns)


### Questions

<details>
  <summary>What are design patterns?</summary>

  Design patterns are standard solutions to common problems in a software design. Each design pattern provides a customized blueprint for exacting problems. As a result, you cannot copy a pattern in your program, but you can use it as a design solution to your problem. The design patterns could be confused with algorithms because both concepts describe standard solutions to some known targets. But while an algorithm has always defined a clear set of actions, a pattern is a more high-level description of a solution.

</details>

<details>
  <summary>Why should patterns be learned?</summary>
  
  The truth is that a programmer can work without knowledge about patterns. Moreover, in this case, he can implement a pattern solution without knowing about it. So, why is it needed to learn them?
  There are a few reasons:
	  1. Firstly, design patterns are a toolkit of solutions to common problems in software design. So, the programmer could solve problems using them.
	  2. Secondly, design patterns are a common language that allows having more effective communication.

</details>

### Creational patterns

#### Links
[Factory Method](https://refactoring.guru/design-patterns/factory-method)
[Abstract Factory](https://refactoring.guru/design-patterns/abstract-factory)
[Builder](https://refactoring.guru/design-patterns/builder)
[Prototype](https://refactoring.guru/design-patterns/prototype)
[Singleton](https://refactoring.guru/design-patterns/singleton)

#### Questions

<details>
  <summary>What is Factory Method?</summary>

  Factory Method is a creational design pattern that provides an interface for creating objects in a superclass but allows subclasses to alter the type of created objects.
  Applicability:
  * Use the factory Method when beforehand unknown types and dependencies of the objects should work.
  * Use the Factory Method for providing users of your library or framework with a way to extend its internal components.
  * Use the Factory Method for saving system resources by reusing the existing exemplars instead of rebuilding them each time.
  Pros:
  * Avoid tight coupling between the creator and the concrete products.
  * Single Responsibility Principle. You can move the product creation code into one place in the program, making the code easier to support.
  * Open/Closed Principle. You can introduce new types of products into the program without breaking existing client code.
  Cons:
  * Each new subclass increases the code complexity. The best-case scenario is when introducing the pattern into an existing hierarchy of creator classes.

</details>

<details>
  <summary>What is Abstract Factory?</summary>

  Abstract Factory is a creational design pattern that lets you produce families of the related objects without specifying their concrete classes.
  Applicability:
  * Use the Abstract Factory when code needs to work with various families of related products but not to depend on the concrete classes of those products - they might be unknown beforehand or be simplified to allow for future extensibility.
  Pros:
  * Be sure that the products from a factory are compatible with each other.
  * Avoid tight coupling between concrete products and client code.
  * Single Responsibility Principle. Extract the product creation code into one place, making the code easier to support.
  * Open/Closed Principle. Introduce new variants of products without breaking existing client code.
  Cons:
  * Each new interface or class increases the complexity of the code.

</details>

<details>
  <summary>What is Builder?</summary>

  Builder is a creational design pattern that lets you construct complex objects step by step. The builder pattern allows producing different types and representations of an object using the same construction code.
  Applicability:
  * Use the Builder pattern to get rid of a 'telescopic constructor'.
  * Use the Builder pattern when an application needs to create different representations of some product, for example, stone and wooden houses.
  * Use the Builder to construct Composite trees or other complex objects.
  Pros:
  * Construct objects step-by-step, defer construction steps or run steps recursively.
  * Reuse the same construction code when building various representations of products.
  * Single Responsibility Principle. Isolate complex construction code from the business logic of the product.
  Cons:
  * The overall complexity of the code increases since the pattern requires creating multiple new classes.

</details>

<details>
  <summary>What is a Prototype?</summary>

  A Prototype is a creational design pattern that lets you copy existing objects without making your code dependent on their classes.
  Applicability:
  * Use the Prototype pattern when there isn't dependency from the concrete classes of copied objects in a code.
  * Use the pattern when you want to reduce the number of subclasses that only differ from the initialization of their respective objects. Somebody could have created these subclasses to be able to create a new one with a specific configuration.
  Pros:
  * Clone objects without coupling to their concrete classes.
  * Get rid of repeated initialization code in favour of cloning pre-built prototypes.
  * Produce complex exemplars more conveniently.
  * Get an alternative to inheritance when dealing with configuration presets.
  Cons:
  * Cloning complex objects that have circular references might be very tricky.

</details>

<details>
  <summary>What is Singleton?</summary>

  Singleton is a creational design pattern that lets you ensure that a class has only one instance while providing a global access point to this instance.
  Applicability:
  * Use the Singleton pattern when a class in your program should have just a single instance available to all clients; for example, a single database object shared by different parts of the program.
  * Use the Singleton pattern when you need stricter control over global variables.
  Pros:
  * You can be sure that a class has only a single instance.
  * You gain a global access point to that instance.
  * The initialization of the singleton object happens during the first call.
  Cons:
  * Single Responsibility Principle. The pattern solves two problems at the time.
  * The Singleton pattern can mask unluck design, for instance, when the program components know too much about each other.
  * The pattern requires special treatment in a multithreaded environment so that multiple threads cannot create a singleton object several times.
  * It may be difficult to unit test the client code because many test frameworks rely on inheritance when producing mock objects. Since the constructor of the singleton class is private and overriding static methods is impossible in most languages, you will need to think of a creative way to mock the singleton.

</details>

### Structural patterns

#### Links

#### Questions

<details>
  <summary>What is Adapter?</summary>

  In progress ...

</details>

<details>
  <summary>What is Bridge?</summary>

  In progress ...

</details>

<details>
  <summary>What is Composite?</summary>

  In progress ...

</details>

<details>
  <summary>What is Decorator?</summary>

  In progress ...

</details>

<details>
  <summary>What is Facade?</summary>

  In progress ...

</details>

<details>
  <summary>What is Flyweight?</summary>

  In progress ...

</details>

<details>
  <summary>What is Proxy?</summary>

  In progress ...

</details>

### Behavioral patterns

#### Links

#### Questions

<details>
  <summary>What is Chain of Responsibility?</summary>

  In progress ...

</details>

<details>
  <summary>What is Command?</summary>

  In progress ...

</details>

<details>
  <summary>What is Iterator?</summary>

  In progress ...

</details>

<details>
  <summary>What is Mediator?</summary>

  In progress ...

</details>

<details>
  <summary>What is Memento?</summary>

  In progress ...

</details>

<details>
  <summary>What is Observer?</summary>

  In progress ...

</details>

<details>
  <summary>What is State?</summary>

  In progress ...

</details>

<details>
  <summary>What is Strategy?</summary>

  In progress ...

</details>

<details>
  <summary>What is Template Method?</summary>

  In progress ...

</details>

<details>
  <summary>What is Visitor?</summary>

  In progress ...

</details>
