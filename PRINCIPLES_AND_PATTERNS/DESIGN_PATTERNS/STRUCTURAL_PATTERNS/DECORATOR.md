# Decorator

### Links

[Refactoring guru / decorator](https://refactoring.guru/design-patterns/decorator)

<details>
  <summary>What is a Decorator?</summary>

Decorator is a structural design pattern that lets you attach new behaviors to objects by placing these objects inside special wrapper objects that contain the behaviors.

</details>

<details>
  <summary>What is a Decorator's Applicability?</summary>

- Use the Decorator pattern when you need to be able to assign extra behaviors to objects at runtime without breaking the code that uses these objects;
- Use the pattern when it’s awkward or not possible to extend an object’s behavior using inheritance.

</details>

<details>
  <summary>What are pros of a Decorator pattern?</summary>

- It is possitble to extend an object’s behavior without making a new subclass;
- It is possitble to add or remove responsibilities from an object at runtime;
- It is possitble to combine several behaviors by wrapping an object into multiple decorators;
- It is possitble to divide a monolithic class that implements many possible variants of behavior into several smaller classes (Single Responsibility Principle).

</details>

<details>
  <summary>What are cons of a Decorator pattern?</summary>

- It’s hard to remove a specific wrapper from the wrappers stack;
- It’s hard to implement a decorator in such a way that its behavior doesn’t depend on the order in the decorators stack;
- The initial configuration code of layers might look pretty ugly.

</details>
