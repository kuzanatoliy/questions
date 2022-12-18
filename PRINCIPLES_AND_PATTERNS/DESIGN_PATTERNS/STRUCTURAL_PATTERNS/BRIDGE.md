# Bridge

<details>
  <summary>What is Bridge?</summary>

The Bridge is a structural design pattern that lets you split a large class or a set of closely related classes into two separate hierarchies - abstraction and implementation - their implementation independent of each other.

Applicability:

- Use the Bridge pattern when you want to divide and organize a class with several functional variants (for example, if the implemented class can work with various database servers).
- Use the pattern when you need to extend a class in several orthogonal (independent) dimensions.
- Use the Bridge if you need to be able to switch implementations at runtime.

Prons:

- You can create platform-independent classes and apps.
- The client code works with high-level abstractions.
- Open/Closed Principle. You can introduce new abstractions and implementations independently from each other.
- Single Responsibility Principle. You can focus on high-level logic in the abstraction and on platform details in the implementation.

Cons:

- You might make the code more complicated by applying the pattern to a highly cohesive class.

[More >>](https://refactoring.guru/design-patterns/bridge)

</details>
