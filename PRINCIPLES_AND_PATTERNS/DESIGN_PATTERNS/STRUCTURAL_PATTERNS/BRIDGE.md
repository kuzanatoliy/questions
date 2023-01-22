# Bridge


### Links

[Refactoring guru / bridge](https://refactoring.guru/design-patterns/bridge)

<details>
  <summary>What is a Bridge?</summary>

Bridge is a structural design pattern that lets you split a large class or a set of closely related classes into two separate hierarchies—abstraction and implementation—which can be developed independently of each other.

</details>

<details>
  <summary>What is a Bridge's Applicability?</summary>

- Use the Bridge pattern when you want to divide and organize a monolithic class that has several variants of some functionality (for example, if the class can work with various database servers);
- Use the pattern when you need to extend a class in several orthogonal (independent) dimensions;
- Use the Bridge if you need to be able to switch implementations at runtime.

</details>

<details>
  <summary>What are pros of a Bridge pattern?</summary>

- It is possible to create platform-independent classes and apps.
- The client code works with high-level abstractions. It isn’t exposed to the platform details.
- It is possible to introduce new abstractions and implementations independently from each other (Open/Closed Principle).
- It is possible to focus on high-level logic in the abstraction and on platform details in the implementation (Single Responsibility Principle).

</details>

<details>
  <summary>What are cons of a Bridge pattern?</summary>

- You might make the code more complicated by applying the pattern to a highly cohesive class.

</details>
