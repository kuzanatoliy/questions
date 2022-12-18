# Factory method

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
