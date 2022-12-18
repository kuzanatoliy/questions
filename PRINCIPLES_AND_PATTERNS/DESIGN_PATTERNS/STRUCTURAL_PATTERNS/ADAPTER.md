# Adapter

<details>
  <summary>What is Adapter?</summary>

The adapter is a structural design pattern that allows objects with incompatible interfaces to collaborate.

Applicability:

- Use the adapter when you want to use some existing class, but its interface is not compatible with the rest of your code.
- Use the pattern for reusing several existing subclasses that lack some functionality, and there is not possible to add it in the superclass.

Prons:

- Single Responsibility Principle. You can separate the interface or data conversion code from the primary business logic of the program.
- Open/Closed Principle. You can introduce new types of adapters into the program without breaking the existing client code, as long as they work with the adapters through the client interface.

Cons:

- The overall complexity of the code increases because it requires introducing a set of new interfaces and classes. From time to time, changing into service is an easier way.

[More >>](https://refactoring.guru/design-patterns/adapter)

</details>
