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
  <summary>What do you know about KISS?</summary>

  In progress ...

</details>

## Design patterns

### Links

### Creational patterns

#### Links
[Factory Method](https://refactoring.guru/design-patterns/factory-method)

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
  <summary>What is Prototype?</summary>

  In progress ...

</details>

<details>
  <summary>What is Singleton?</summary>

  In progress ...

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
