# Command

<details>
  <summary>What is Command?</summary>

It is a behavioural design pattern that turns a request into a stand-alone object that contains all information about it. This transformation lets you pass requests to method arguments, delay or queue a request execution, and support undoable operations.

Applicability:

- Use the Command pattern when you want to parametrize objects with operations.
- Use the Command pattern when you want to queue operations, schedule their execution, or execute them remotely.
- Use the Command pattern when an application can reverse operations.

Prons:

- Single Responsibility Principle. It is possible to decouple classes that invoke operations from them that perform these operations.
- Open/Closed Principle. You can introduce new commands into the app without breaking existing client code.
- You can implement undo/redo.
- You can implement deferred execution of operations.
- You can assemble a set of simple commands into a complex one.

Cons:

- The code may become more complicated since introducing a whole new layer between senders and receivers.

[More >>](https://refactoring.guru/design-patterns/command)

</details>
