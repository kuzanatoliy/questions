# Abstract factory

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
