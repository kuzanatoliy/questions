# Decorator

<details>
  <summary>What is a Decorator?</summary>

The decorator is a structural design pattern that lets you attach new behaviours to objects by placing these objects inside specialized wrapper objects that contain the behaviours.

Applicability:

- Use the Decorator pattern when it is possible to increase behaviours at runtime without breaking the code that uses these objects.
- Use it when it is impossible to extend behaviour using inheritance.

Prons:

- It is possible to extend a behaviour without making a new subclass.
- It is possible to add or remove responsibilities from an object at runtime.
- It is possible to combine several behaviours by wrapping an object into multiple decorators.
- Single Responsibility Principle. You can divide a monolithic class that implements many possible variants of behaviour into several smaller ones.

Cons:

- It is hard to remove a specific wrapper from the wrappers stack.
- It is hard to implement a decorator with independent behaviour from the stack.
- The initial configuration code of layers might look pretty ugly.

[More >>](https://refactoring.guru/design-patterns/decorator)

</details>
