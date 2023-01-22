# Command

### Links

[Refactoring guru / command](https://refactoring.guru/design-patterns/command)

<details>
  <summary>What is a Command?</summary>

Command is a behavioral design pattern that turns a request into a stand-alone object that contains all information about the request. This transformation lets you pass requests as a method arguments, delay or queue a request’s execution, and support undoable operations.

</details>

<details>
  <summary>What is a Command's Applicability?</summary>

- Use the Command pattern when you want to parametrize objects with operations;
- Use the Command pattern when you want to queue operations, schedule their execution, or execute them remotely;
- Use the Command pattern when you want to implement reversible operations.

</details>

<details>
  <summary>What are pros of a Command pattern?</summary>

- It is possible to decouple classes that invoke operations from classes that perform these operations (Single Responsibility Principle);
- It is possible to introduce new commands into the app without breaking existing client code (Open/Closed Principle);
- It is possible to implement undo/redo;
- It is possible to implement deferred execution of operations;
- It is possible to assemble a set of simple commands into a complex one.

</details>

<details>
  <summary>What are cons of a Proxy pattern?</summary>

- The code may become more complicated since you’re introducing a whole new layer between senders and receivers.

</details>
