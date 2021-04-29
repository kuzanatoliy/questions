# Principles and patterns

## SOLID

<details>
  <summary>What is SOLID?</summary>

  The single responsibility principle - each class should have only one responsibility that encapsulates in this class.
  The open-closed principle - each entity should be open for expansion and be closed for modification.
  The Liskov substitution principle - any subclass should supplement the parent class but not change it.
  The interface segregation principle - a few separate interfaces are better than one combined interface.
  The dependency inversion principle - dependencies should be only on abstractions.

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
[Adapter](https://refactoring.guru/design-patterns/adapter)
[Bridge](https://refactoring.guru/design-patterns/bridge)
[Composite](https://refactoring.guru/design-patterns/composite)
[Decorator](https://refactoring.guru/design-patterns/decorator)
[Facade](https://refactoring.guru/design-patterns/facade)
[Flyweight](https://refactoring.guru/design-patterns/flyweight)
[Proxy](https://refactoring.guru/design-patterns/proxy)

#### Questions

<details>
  <summary>What is Adapter?</summary>

  The adapter is a structural design pattern that allows objects with incompatible interfaces to collaborate.
  Applicability:
  * Use the adapter when you want to use some existing class, but its interface is not compatible with the rest of your code.
  * Use the pattern for reusing several existing subclasses that lack some functionality, and there is not possible to add it in the superclass.
  Prons:
  * Single Responsibility Principle. You can separate the interface or data conversion code from the primary business logic of the program.
  * Open/Closed Principle. You can introduce new types of adapters into the program without breaking the existing client code, as long as they work with the adapters through the client interface.
  Cons:
  * The overall complexity of the code increases because it requires introducing a set of new interfaces and classes. From time to time, changing into service is an easier way.

</details>

<details>
  <summary>What is Bridge?</summary>

  The Bridge is a structural design pattern that lets you split a large class or a set of closely related classes into two separate hierarchies - abstraction and implementation - their implementation independent of each other.
  Applicability:
  * Use the Bridge pattern when you want to divide and organize a class with several functional variants (for example, if the implemented class can work with various database servers).
  * Use the pattern when you need to extend a class in several orthogonal (independent) dimensions.
  * Use the Bridge if you need to be able to switch implementations at runtime.
  Prons:
  * You can create platform-independent classes and apps.
  * The client code works with high-level abstractions.
  * Open/Closed Principle. You can introduce new abstractions and implementations independently from each other.
  * Single Responsibility Principle. You can focus on high-level logic in the abstraction and on platform details in the implementation.
  Cons:
  * You might make the code more complicated by applying the pattern to a highly cohesive class.

</details>

<details>
  <summary>What is Composite?</summary>

  Composite is a structural design pattern that lets you compose objects into tree structures and then work with these structures as if they were individual objects.
  Applicability:
  * Use the Composite pattern when you have to implement a tree-like object structure.
  * Use it when you want the client code to treat both simple and complex elements uniformly.
  Prons:
  * It is possible to work with complex tree structures more conveniently: use polymorphism and recursion to your advantage.
  * Open/Closed Principle. You can introduce new element types into the app without breaking the existing code, which now works with the object tree.
  Cons:
  * It is difficult to provide a shared interface for classes whose functionality differs too much. In base scenarios, there is possible to overgeneralize the component interface, making it harder to comprehend.

</details>

<details>
  <summary>What is a Decorator?</summary>

  The decorator is a structural design pattern that lets you attach new behaviours to objects by placing these objects inside specialized wrapper objects that contain the behaviours.
  Applicability:
  * Use the Decorator pattern when it is possible to increase behaviours at runtime without breaking the code that uses these objects.
  * Use it when it is impossible to extend behaviour using inheritance.
  Prons:
  * It is possible to extend a behaviour without making a new subclass.
  * It is possible to add or remove responsibilities from an object at runtime.
  * It is possible to combine several behaviours by wrapping an object into multiple decorators.
  * Single Responsibility Principle. You can divide a monolithic class that implements many possible variants of behaviour into several smaller ones.
  Cons:
  * It is hard to remove a specific wrapper from the wrappers stack.
  * It is hard to implement a decorator with independent behaviour from the stack.
  * The initial configuration code of layers might look pretty ugly.

</details>

<details>
  <summary>What is a Facade?</summary>

  It is a structural design pattern that provides a simplified interface to a library, a framework, or any other complex set of classes.
  Applicability:
  * Use the Facade pattern when you need to have a limited but straightforward interface to a complex subsystem.
  * Use the Facade when you want to structure a subsystem into layers.
  Prons:
  * It is possible to isolate your code from the complexity of a subsystem.
  Cons:
  * A facade can become a god object coupled to all classes of an app.

</details>

<details>
  <summary>What is Flyweight?</summary>

  What is Flyweight?
  Flyweight is a structural design pattern that lets you fit more objects into the available amount of RAM by sharing common parts of the state between multiple exemplars instead of keeping all of the data in each object.
  Applicability:
  * Use the Flyweight pattern only when it is needed to optimize used RAM.
  Prons:
  * It is possible to save lots of RAM, assuming your program has tons of similar objects.
  Cons:
  * It is possible to trade RAM over CPU cycles when some context data needs recalculation each time somebody calls a flyweight method.
  * The code becomes much more complicated. New team members will always be wondering about the state.

</details>

<details>
  <summary>What is Proxy?</summary>

  What is a Proxy?
  Proxy is a structural design pattern that provides a substitute or placeholder for another object. A proxy controls access to the original one, allowing it to perform something either before or after the request gets through to the original one.
  Applicability:
  * Lazy initialization.
  * Access control (protection proxy).
  * Logging requests (logging proxy).
  * Caching request results (caching proxy).
  * Smart reference.
  Prons:
  * It is possible to control the service object without clients knowing about it.
  * It is possible to manage the lifecycle of the service object when clients do not care about it.
  * The proxy works even if the service object is not ready or is not available.
  * Open/Closed Principle. You can introduce new proxies without changing the service or clients.
  Cons:
  * The code may become more complicated since you need to introduce a lot of new classes.

</details>

### Behavioral patterns

#### Links
[Chain of responsibility](https://refactoring.guru/design-patterns/chain-of-responsibility)
[Command](https://refactoring.guru/design-patterns/command)
[Iterator](https://refactoring.guru/design-patterns/iterator)
[Mediator](https://refactoring.guru/design-patterns/mediator)
[Memento](https://refactoring.guru/design-patterns/memento)
[Observer](https://refactoring.guru/design-patterns/observer)
[State](https://refactoring.guru/design-patterns/state)
[Strategy](https://refactoring.guru/design-patterns/strategy)
[Template method](https://refactoring.guru/design-patterns/template-method)
[Visitor](https://refactoring.guru/design-patterns/visitor)

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
