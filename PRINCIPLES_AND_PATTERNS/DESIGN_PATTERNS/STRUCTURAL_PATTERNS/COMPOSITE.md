# Composite

<details>
  <summary>What is Composite?</summary>

Composite is a structural design pattern that lets you compose objects into tree structures and then work with these structures as if they were individual objects.

Applicability:

- Use the Composite pattern when you have to implement a tree-like object structure.
- Use it when you want the client code to treat both simple and complex elements uniformly.

Prons:

- It is possible to work with complex tree structures more conveniently: use polymorphism and recursion to your advantage.
- Open/Closed Principle. You can introduce new element types into the app without breaking the existing code, which now works with the object tree.

Cons:

- It is difficult to provide a shared interface for classes whose functionality differs too much. In base scenarios, there is possible to overgeneralize the component interface, making it harder to comprehend.

[More >>](https://refactoring.guru/design-patterns/composite)

</details>
