# Observer

<details>
  <summary>What is Observer?</summary>

It is a behavioural design pattern that lets you define a subscription mechanism to notify multiple objects about any events.

Applicability:

- Use the Observer pattern when changes to the state of one object may require changing other ones, and the set of the object is unknown beforehand or changes dynamically.
- Use the pattern when some parts in an app must observe others, but only for a limited time or in specific cases.

Prons:

- Open/Closed Principle. You can introduce new subscriber classes without changing the code (and vice versa if there is a publisher interface).
- You can establish relations between objects at runtime.

Cons:

- Subscribers get notifications in random order.

[More >>](https://refactoring.guru/design-patterns/observer)

</details>
