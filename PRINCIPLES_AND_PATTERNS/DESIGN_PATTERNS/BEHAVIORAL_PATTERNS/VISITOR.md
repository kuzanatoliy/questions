# Visitor

<details>
  <summary>What is Visitor?</summary>

It is a behavioural design pattern that lets you separate algorithms from the objects on which they operate.

Applicability:

- Use the Visitor when you need to operate on all elements of a complex object structure (for example, an object tree).
- Use the Visitor to clean up the business logic of auxiliary behaviours.
- Use the pattern when a behaviour makes sense only in some classes of a class hierarchy, but not in others.

Prons:

- Open/Closed Principle. You can introduce a new behaviour that can work with objects of different classes without changing these classes.
- Single Responsibility Principle. You can move multiple versions of the same behaviour into the same class.
- A visitor object can accumulate some information while working with various. It might be handy when you want to traverse some complex object structure, such as an object tree, and apply one to each object of this structure.

Cons:

- You need to update all visitors each time a class gets added to or removed from the element hierarchy.
- Visitors might lack the necessary access to the private fields and methods of the elements

[More >>](https://refactoring.guru/design-patterns/visitor)

</details>
