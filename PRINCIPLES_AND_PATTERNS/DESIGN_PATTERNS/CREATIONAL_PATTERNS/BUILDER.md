# Builder

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
