# Momento

<details>
  <summary>What is Memento?</summary>

Memento is a behavioural design pattern that lets you save and restore the previous state of an object without revealing the details of its implementation.

Applicability:

- Use the Memento pattern when you want to produce snapshots of the object state for the ability to restore a previous state of the object.
- Use it when direct access to the object fields/getters/setters violates its encapsulation.

Prons:

- It is possible to produce snapshots of the state without violating its encapsulation.
- It is possible to simplify the code by letting the caretaker maintain the history of the state.

Cons:

- The app might consume lots of RAM if clients create mementoes too often.
- Caretakers should track the lifecycle to be able to destroy obsolete mementoes.
- Most dynamic programming languages, such as PHP, Python and JavaScript, don't guarantee that the state within the Memento stays untouched.

[More >>](https://refactoring.guru/design-patterns/memento)

</details>
