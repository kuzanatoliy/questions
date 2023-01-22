# Mediator

### Links

[Refactoring guru / mediator](https://refactoring.guru/design-patterns/mediator)

<details>
  <summary>What is a Mediator?</summary>

Mediator is a behavioral design pattern that lets you reduce chaotic dependencies between objects. The pattern restricts direct communications between the objects and forces them to collaborate only via a mediator object.

</details>

<details>
  <summary>What is a Mediator's Applicability?</summary>

- Use the Mediator pattern when it’s hard to change some of the classes because they are tightly coupled to a bunch of other classes;
- Use the pattern when you can’t reuse a component in a different program because it’s too dependent on other components;
- Use the Mediator when you find yourself creating tons of component subclasses just to reuse some basic behavior in various contexts.

</details>

<details>
  <summary>What are pros of a Mediator pattern?</summary>

- It is possible to extract the communications between various components into a single place, making it easier to comprehend and maintain (Single Responsibility Principle);
- It is possible to introduce new mediators without having to change the actual components (Open/Closed Principle);
- It is possible to reduce coupling between various components of a program;
- It is possible to reuse individual components more easily.

</details>

<details>
  <summary>What are cons of a Proxy pattern?</summary>

- Over time a mediator can evolve into a God Object.

</details>
