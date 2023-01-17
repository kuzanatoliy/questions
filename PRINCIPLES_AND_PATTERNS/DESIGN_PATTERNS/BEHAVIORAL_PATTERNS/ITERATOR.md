# Iterator

### Links

[Refactoring guru / iterator](https://refactoring.guru/design-patterns/iterator)

<details>
  <summary>What is a Iterator?</summary>

Iterator is a behavioral design pattern that lets you traverse elements of a collection without exposing its underlying representation (list, stack, tree, etc.).

</details>

<details>
  <summary>What is a Iterator's Applicability?</summary>

- Use the Iterator pattern when your collection has a complex data structure under the hood, but you want to hide its complexity from clients (either for convenience or security reasons);
- Use the pattern to reduce duplication of the traversal code across your appc;
- Use the Iterator when you want your code to be able to traverse different data structures or when types of these structures are unknown beforehand.

</details>

<details>
  <summary>What are pros of a Iterator pattern?</summary>

- It is possitble to clean up the client code and the collections by extracting bulky traversal algorithms into separate classes (Single Responsibility Principle);
- It is possitble to implement new types of collections and iterators and pass them to existing code without breaking anything (Open/Closed Principle);
- It is possitble to iterate over the same collection in parallel because each iterator object contains its own iteration state;
- For the same reason, you can delay an iteration and continue it when needed.

</details>

<details>
  <summary>What are cons of a Proxy pattern?</summary>

- Applying the pattern can be an overkill if your app only works with simple collections;
- Using an iterator may be less efficient than going through elements of some specialized collections directly.

</details>
