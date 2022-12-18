# Builder

### Links

[Refactoring guru / builder](https://refactoring.guru/design-patterns/builder)

<details>
  <summary>What is Builder?</summary>

Builder is a creational design pattern that lets you construct complex objects step by step. The builder pattern allows producing different types and representations of an object using the same construction code.

</details>

<details>
  <summary>What is a Builder's Applicability?</summary>

- Avoid using a lot of constructor variants;
- Use the Builder pattern when an application needs to create different representations of some product, for example, stone and wooden houses;
- Use for constructing Composite trees or other complex objects.

</details>

<details>
  <summary>What are pros of a Builder pattern?</summary>

- Construct objects step-by-step, defer construction steps or run steps recursively;
- Reuse the same construction code when building various representations of products;
- Single Responsibility Principle. Isolate complex construction code from the business logic of the product.

</details>

<details>
  <summary>What are cons of a Builder pattern?</summary>

- The overall complexity of the code increases since the pattern requires creating multiple new classes;
- The clients will be bind with specific classes.

</details>

### Connections

- A [Factory method](FACTORY_METHOD.md) could evolve into an [Abstract factory](ABSTRACT_FACTORY.md), a [Prototype](PROTOTYPE.md), a **Builder**;
- The **Builder** concentrate on building complecated objects step by step. The [Abstract factory](ABSTRACT_FACTORY.md) concentrates on producing families;
- The **Builder** allows to build a [Composite](../STRUCTURAL_PATTERNS/COMPOSITE.md) step-by-step;
- The **Builder** could be implemented like a [Bridge](../STRUCTURAL_PATTERNS/BRIDGE.md);
- The [Facade](../STRUCTURAL_PATTERNS/FACADE.md), a [Flyweight](../STRUCTURAL_PATTERNS/FLYWEIGHT.md), [Abstract factory](ABSTRACT_FACTORY.md), the **Builder**, the [Prototype](PROTOTYPE.md) might be implemented like a [Singleton](SINGLETON.md).
