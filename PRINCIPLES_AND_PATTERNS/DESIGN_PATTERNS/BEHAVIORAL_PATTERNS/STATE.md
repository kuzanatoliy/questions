# State

### Links

[Refactoring guru / state](https://refactoring.guru/design-patterns/state)

<details>
  <summary>What is a State?</summary>

State is a behavioral design pattern that lets an object alter its behavior when its internal state changes. It appears as if the object changed its class.

</details>

<details>
  <summary>What is a State's Applicability?</summary>

- Use the State pattern when you have an object that behaves differently depending on its current state, the number of states is enormous, and the state-specific code changes frequently;
- Use the pattern when you have a class polluted with massive conditionals that alter how the class behaves according to the current values of the class’s fields;
- Use State when you have a lot of duplicate code across similar states and transitions of a condition-based state machine.

</details>

<details>
  <summary>What are pros of a State pattern?</summary>

- Organize the code related to particular states into separate classes (Single Responsibility Principle);
- Introduce new states without changing existing state classes or the context (Open/Closed Principle);
- Simplify the code of the context by eliminating bulky state machine conditionals.

</details>

<details>
  <summary>What are cons of a Proxy pattern?</summary>

- Applying the pattern can be overkill if a state machine has only a few states or rarely changes.

</details>
