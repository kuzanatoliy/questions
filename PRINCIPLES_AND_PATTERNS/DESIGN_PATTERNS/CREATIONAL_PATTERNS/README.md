# Creational patterns

[Singleton](SINGLETON.md)

<details>
  <summary>What is Factory Method?</summary>

Factory Method is a creational design pattern that provides an interface for creating objects in a superclass but allows subclasses to alter the type of created objects.

Applicability:

- Use the factory Method when beforehand unknown types and dependencies of the objects should work.
- Use the Factory Method for providing users of your library or framework with a way to extend its internal components.
- Use the Factory Method for saving system resources by reusing the existing exemplars instead of rebuilding them each time.

Pros:

- Avoid tight coupling between the creator and the concrete products.
- Single Responsibility Principle. You can move the product creation code into one place in the program, making the code easier to support.
- Open/Closed Principle. You can introduce new types of products into the program without breaking existing client code.

Cons:

- Each new subclass increases the code complexity. The best-case scenario is when introducing the pattern into an existing hierarchy of creator classes.

[More >>](https://refactoring.guru/design-patterns/factory-method)

</details>

<details>
  <summary>What is Abstract Factory?</summary>

Abstract Factory is a creational design pattern that lets you produce families of the related objects without specifying their concrete classes.

Applicability:

- Use the Abstract Factory when code needs to work with various families of related products but not to depend on the concrete classes of those products - they might be unknown beforehand or be simplified to allow for future extensibility.

Pros:

- Be sure that the products from a factory are compatible with each other.
- Avoid tight coupling between concrete products and client code.
- Single Responsibility Principle. Extract the product creation code into one place, making the code easier to support.
- Open/Closed Principle. Introduce new variants of products without breaking existing client code.

Cons:

- Each new interface or class increases the complexity of the code.

[More >>](https://refactoring.guru/design-patterns/abstract-factory)

</details>

<details>
  <summary>What is Builder?</summary>

Builder is a creational design pattern that lets you construct complex objects step by step. The builder pattern allows producing different types and representations of an object using the same construction code.

Applicability:

- Use the Builder pattern to get rid of a 'telescopic constructor'.
- Use the Builder pattern when an application needs to create different representations of some product, for example, stone and wooden houses.
- Use the Builder to construct Composite trees or other complex objects.

Pros:

- Construct objects step-by-step, defer construction steps or run steps recursively.
- Reuse the same construction code when building various representations of products.
- Single Responsibility Principle. Isolate complex construction code from the business logic of the product.

Cons:

- The overall complexity of the code increases since the pattern requires creating multiple new classes.

[More >>](https://refactoring.guru/design-patterns/builder)

</details>

<details>
  <summary>What is a Prototype?</summary>

A Prototype is a creational design pattern that lets you copy existing objects without making your code dependent on their classes.

Applicability:

- Use the Prototype pattern when there isn't dependency from the concrete classes of copied objects in a code.
- Use the pattern when you want to reduce the number of subclasses that only differ from the initialization of their respective objects. Somebody could have created these subclasses to be able to create a new one with a specific configuration.

Pros:

- Clone objects without coupling to their concrete classes.
- Get rid of repeated initialization code in favour of cloning pre-built prototypes.
- Produce complex exemplars more conveniently.
- Get an alternative to inheritance when dealing with configuration presets.

Cons:

- Cloning complex objects that have circular references might be very tricky.

[More >>](https://refactoring.guru/design-patterns/prototype)

</details>

