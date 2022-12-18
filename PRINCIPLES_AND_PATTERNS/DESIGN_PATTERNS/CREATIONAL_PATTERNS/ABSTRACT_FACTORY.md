# Abstract factory

### Links

[Refactoring guru / abstract factory](https://refactoring.guru/design-patterns/abstract-factory)

<details>
  <summary>What is Abstract Factory?</summary>

Abstract Factory is a creational design pattern that lets you produce families of the related objects without specifying their concrete classes.

</details>

<details>
  <summary>What is an Abstract factory' Applicability?</summary>

- Use when a business logic requires working with different families of related products that aren't depend on the concreate implementations;
- Use when application already uses a [factory method](FACTORY_METHOD.md) and new functionality requires new types.

</details>

<details>
  <summary>What are pros of an Abstract factory pattern?</summary>

- Guarantee a connection between created products;
- Allows a client code to avoid a hard linking with a class implementation;
- Extract the product creation code into one place, making the code easier to support (The single responsibility principle);
- Introduce new types of products into the program without breaking existing client code (Open/Closed Principle).

</details>

<details>
  <summary>What are cons of an Abstract factory pattern?</summary>

- Each new interface or class increases the complexity of the code;
- Requires all types into each variant.

</details>

### Connections

- A [Factory method](FACTORY_METHOD.md) could evolve into the **Abstract factory**, a [Prototype](PROTOTYPE.md), a [Builder](BUILDER.md);
- A [Builder](BUILDER.md) concentrate on building complecated objects step by step. The **Abstract factory** concentrates on producing families;
- The **Abstract factory** could be implemented by the [Factory method](FACTORY_METHOD.md) or the [Prototype](PROTOTYPE.md);
- The **Abstract factory** could be used instead of a [Facade](../STRUCTURAL_PATTERNS/FACADE.md);
- The **Abstract factory** could be used with a [Bridge](../STRUCTURAL_PATTERNS/BRIDGE.md);
- The [Facade](../STRUCTURAL_PATTERNS/FACADE.md), a [Flyweight](../STRUCTURAL_PATTERNS/FLYWEIGHT.md), **Abstract factory**, the [Builder](Builder.md), the [Prototype](PROTOTYPE.md) might be implemented like **Singleton**.
