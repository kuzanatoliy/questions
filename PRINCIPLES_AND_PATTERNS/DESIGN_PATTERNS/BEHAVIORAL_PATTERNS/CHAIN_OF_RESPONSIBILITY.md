# Chain of Responsibility

<details>
  <summary>What is Chain of Responsibility?</summary>

Cin of Responsibility is a behavioural design pattern that lets you pass requests along a chain of handlers. Each handler decides thao process the request or move it on to the next handler in the chain.

Applicability:

- Use the Chain of Responsibility pattern when an expected program process different kinds of requests in various ways, but the exact types of requests and their sequences are unknown beforehand.
- Use it when it is essential to execute several handlers in a particular order.
- Use the CoR pattern when the set of handlers and their order are supposed to change at runtime.

Prons:

- You can control the order of request handling.
- Single Responsibility Principle. It is possible to decouple classes that invoke operations from them.
- Open/Closed Principle. You can introduce new handlers into the app without breaking the existing client code.

Cons:

- Some requests may end up unhandled.

[More >>](https://refactoring.guru/design-patterns/chain-of-responsibility)

</details>
