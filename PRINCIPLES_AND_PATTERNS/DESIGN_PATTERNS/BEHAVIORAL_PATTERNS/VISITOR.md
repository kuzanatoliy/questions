# Visitor

### Links

[Refactoring guru / visitor](https://refactoring.guru/design-patterns/visitor)

<details>
  <summary>What is a Visitor?</summary>

Visitor is a behavioral design pattern that lets you separate algorithms from the objects on which they operate.

</details>

<details>
  <summary>What is a Visitor's Applicability?</summary>

- Use the Visitor when you need to perform an operation on all elements of a complex object structure (for example, an object tree);
- Use the Visitor to clean up the business logic of auxiliary behaviors;
- Use the pattern when a behavior makes sense only in some classes of a class hierarchy, but not in others.

</details>

<details>
  <summary>What are pros of a Visitor pattern?</summary>

- Open/Closed Principle. You can introduce a new behavior that can work with objects of different classes without changing these classes;
- Single Responsibility Principle. You can move multiple versions of the same behavior into the same class;
- A visitor object can accumulate some useful information while working with various objects. This might be handy when you want to traverse some complex object structure, such as an object tree, and apply the visitor to each object of this structure.

</details>

<details>
  <summary>What are cons of a Proxy pattern?</summary>

- You need to update all visitors each time a class gets added to or removed from the element hierarchy;
- Visitors might lack the necessary access to the private fields and methods of the elements that they’re supposed to work with.

</details>
