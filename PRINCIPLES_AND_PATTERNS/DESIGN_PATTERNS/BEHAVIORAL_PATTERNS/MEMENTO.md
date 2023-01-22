# Momento

### Links

[Refactoring guru / momento](https://refactoring.guru/design-patterns/momento)

<details>
  <summary>What is a Momento?</summary>

Memento is a behavioral design pattern that lets you save and restore the previous state of an object without revealing the details of its implementation.

</details>

<details>
  <summary>What is a Momento's Applicability?</summary>

- Use the Memento pattern when you want to produce snapshots of the object’s state to be able to restore a previous state of the object;
- Use the pattern when direct access to the object’s fields/getters/setters violates its encapsulation.

</details>

<details>
  <summary>What are pros of a Momento pattern?</summary>

- It is possible to produce snapshots of the object’s state without violating its encapsulation;
- It is possible to simplify the originator’s code by letting the caretaker maintain the history of the originator’s state.

</details>

<details>
  <summary>What are cons of a Proxy pattern?</summary>

- The app might consume lots of RAM if clients create mementos too often;
- Caretakers should track the originator’s lifecycle to be able to destroy obsolete mementos;
- Most dynamic programming languages, such as PHP, Python and JavaScript, can’t guarantee that the state within the memento stays untouched.

</details>
