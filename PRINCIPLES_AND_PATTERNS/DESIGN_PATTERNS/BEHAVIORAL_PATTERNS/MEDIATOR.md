# Mediator

<details>
  <summary>What is Mediator?</summary>

The Mediator is a behavioural design pattern that lets to reduce chaotic dependencies between objects. It restricts direct communications between exemplars and forces those to collaborate only via a mediator.

Applicability:

- Use the Mediator pattern when it is hard to change some of the classes.
- Use it when it is possible to reuse a component in a different program.
- Use the Mediator when you find yourself creating tons of component subclasses.

Prons:

- Single Responsibility Principle. It is possible to extract the communications between various components into a single place, making it easier to comprehend and maintain.
- Open/Closed Principle. It is possible to introduce new mediators without having to change the components.
- It is possible to reduce coupling between various components of a program.
- It is possible to reuse individual components easier.

Cons:

- Over time a mediator can evolve into a God Object.

[More >>](https://refactoring.guru/design-patterns/mediator)

</details>
