# Chain of Responsibility

### Links

[Refactoring guru / chain of responsibility](https://refactoring.guru/design-patterns/chain-of-responsibility)

<details>
  <summary>What is a Chain of Responsibility?</summary>

Chain of Responsibility is a behavioral design pattern that lets you pass requests along a chain of handlers. Upon receiving a request, each handler decides either to process the request or to pass it to the next handler in the chain.

</details>

<details>
  <summary>What is a Chain of Responsibility's Applicability?</summary>

- Use the Chain of Responsibility pattern when your program is expected to process different kinds of requests in various ways, but the exact types of requests and their sequences are unknown beforehand;
- Use the pattern when it’s essential to execute several handlers in a particular order;
- Use the CoR pattern when the set of handlers and their order are supposed to change at runtime.

</details>

<details>
  <summary>What are pros of a Chain of Responsibility pattern?</summary>

- It is possible to control the order of request handling;
- It is possible to decouple classes that invoke operations from classes that perform operations (Single Responsibility Principle);
- It is possible to introduce new handlers into the app without breaking the existing client code (Open/Closed Principle).

</details>

<details>
  <summary>What are cons of a Chain of Responsibility pattern?</summary>

- Some requests may end up unhandled.

</details>
