# Factory method

### Links

[Refactoring guru / factory method](https://refactoring.guru/design-patterns/factory-method)

### Questions

<details>
  <summary>What is Factory Method?</summary>

Factory Method is a creational design pattern that provides an interface for creating objects in a superclass but allows subclasses to alter the type of created objects.

</details>

<details>
  <summary>What is a Factory Method's Applicability?</summary>

- Use when beforehand unknown types and dependencies of the objects should work;
- Use for providing users of your library or framework with a way to extend its internal components;
- Use for saving system resources by reusing the existing exemplars instead of rebuilding them each time.

</details>

<details>
  <summary>What are pros of a Factory Method?</summary>

- Allows to avoid a tight coupling between the creator and the concrete products;
- It is possible to move the product creation code into one place in the program, making the code easier to support (The Single responsibility principle);
- It is possible to introduce new types of products into the program without breaking existing client code (Open/Closed Principle).

</details>

<details>
  <summary>What are cons of a Factory Method?</summary>

- Each new subclass increases the code complexity. The best-case scenario is when introducing the pattern into an existing hierarchy of creator classes

</details>
