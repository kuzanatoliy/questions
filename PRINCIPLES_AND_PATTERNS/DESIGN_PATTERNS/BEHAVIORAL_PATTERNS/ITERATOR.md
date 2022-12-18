# Iterator

<details>
  <summary>What is Iterator?</summary>

Iterator is a behavioural design pattern that lets you traverse elements of a collection without exposing its underlying representation (list, stack, tree, etc.).

Applicability:

- Use the Iterator pattern when element collection has a complex data structure under the hood, but you want to hide its complexity from clients (either for convenience or security reasons).
- Use the pattern to reduce duplication of the traversal code across your app.
- Use the Iterator when it is possible to traverse different data structures or when types of these structures are unknown beforehand.

Prons:

- Single Responsibility Principle. You can clean up the client code and the collections by extracting bulky traversal algorithms into separate classes.
- Open/Closed Principle. You can implement new types of collections and iterators and pass them to existing code without breaking anything.
- It is possible to iterate over the same collection in parallel because each iterative object contains its iteration state.
- For the same reason, it is possible to delay an iteration and continue it when needed.

Cons:

- Applying the pattern can be overkill if your app only works with simple collections.
- Using an iterator may be less efficient than going through elements of some specialized structure.

[More >>](https://refactoring.guru/design-patterns/iterator)

</details>
