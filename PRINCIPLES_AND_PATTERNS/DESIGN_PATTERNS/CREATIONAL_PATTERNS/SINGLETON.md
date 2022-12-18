# Singleton

### Links

[Refactoring guru / singleton](https://refactoring.guru/design-patterns/singleton)

### Questions

<details>
  <summary>What is a Singleton?</summary>

Singleton is a creational design pattern that guarantee that a class or an entity has only one instance and provide global access point.

</details>

<details>
  <summary>What problems does a Singleton solve?</summary>

1. Guarantee that exist only one instance

For example, it could be useful for getting access to common source like a data base

2. Provide a global access point

It is not only global variable. It is possible to change global variable from other part of the code base.

</details>

<details>
  <summary>What is a Singleton's Applicability?</summary>S

- When an application should contain only one instance for some functionality that is available for all clients;
- When it is needed to get more control for global variables.

</details>

<details>
  <summary>What are pros of a Singleton pattern?</summary>

- Guarantee that exist only one instance;
- Provide a global access point;
- Implements lazy initialization of a singleton object.

</details>

<details>
  <summary>What are cons of a Singleton pattern?</summary>

- Break a single responsibility principle. The pattern solves two problems at the time;
- Mask unluck design, for instance, when the program components know too much about each other;
- Multithreading. Multiple threads shouldn't  create a singleton object several times;
- Require a permanent creation of the mock-objects during unit-testing process.

</details>

### Connections

A [Facade](../STRUCTURAL_PATTERNS/FACADE.md), a [Flyweight](../STRUCTURAL_PATTERNS/FLYWEIGHT.md), an [Abstract factory](ABSTRACT_FACTORY.md), a [Builder](Builder.md), a [Prototype](PROTOTYPE.md) might be implemented like **Singleton**.
