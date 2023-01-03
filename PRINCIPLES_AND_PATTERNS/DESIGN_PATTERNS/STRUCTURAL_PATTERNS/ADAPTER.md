# Adapter

### Links

[Refactoring guru / adapter](https://refactoring.guru/design-patterns/adapter)

<details>
  <summary>What is an Adapter?</summary>

Adapter is a structural design pattern that allows objects with incompatible interfaces to collaborate.

</details>

<details>
  <summary>What is an Adapter's Applicability?</summary>

- Use the Adapter class when you want to use some existing class, but its interface isn’t compatible with the rest of your code;
- Use the pattern when you want to reuse several existing subclasses that lack some common functionality that can’t be added to the superclass.

</details>

<details>
  <summary>What are pros of an Adapter pattern?</summary>

- It is possible to separate the interface or data conversion code from the primary business logic of the program (Single Responsibility Principle).
- It is possible to introduce new types of adapters into the program without breaking the existing client code, as long as they work with the adapters through the client interface (Open/Closed Principle).

</details>

<details>
  <summary>What are cons of an Adapter pattern?</summary>

- The overall complexity of the code increases because you need to introduce a set of new interfaces and classes. Sometimes it’s simpler just to change the service class so that it matches the rest of your code.

</details>
