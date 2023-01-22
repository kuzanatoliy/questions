# Composite

### Links

[Refactoring guru / composite](https://refactoring.guru/design-patterns/composite)

<details>
  <summary>What is a Composite?</summary>

Composite is a structural design pattern that lets you compose objects into tree structures and then work with these structures as if they were individual objects.

</details>

<details>
  <summary>What is a Composite's Applicability?</summary>

- Use the Composite pattern when you have to implement a tree-like object structure;
- Use the pattern when you want the client code to treat both simple and complex elements uniformly.

</details>

<details>
  <summary>What are pros of a Composite pattern?</summary>

- It is possible to work with complex tree structures more conveniently: use polymorphism and recursion to your advantage.
- It is possible to introduce new element types into the app without breaking the existing code, which now works with the object tree (Open/Closed Principle).

</details>

<details>
  <summary>What are cons of a Composite pattern?</summary>

- It might be difficult to provide a common interface for classes whose functionality differs too much. In certain scenarios, you’d need to overgeneralize the component interface, making it harder to comprehend.

</details>
