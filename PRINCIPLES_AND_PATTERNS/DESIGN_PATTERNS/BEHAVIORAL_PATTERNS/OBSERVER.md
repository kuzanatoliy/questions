# Observer

### Links

[Refactoring guru / observer](https://refactoring.guru/design-patterns/observer)

<details>
  <summary>What is an Observer?</summary>

Observer is a behavioral design pattern that lets you define a subscription mechanism to notify multiple objects about any events that happen to the object they’re observing.

</details>

<details>
  <summary>What is an Observer's Applicability?</summary>

- Use the Observer pattern when changes to the state of one object may require changing other objects, and the actual set of objects is unknown beforehand or changes dynamically;
- Use the pattern when some objects in your app must observe others, but only for a limited time or in specific cases.

</details>

<details>
  <summary>What are pros of an Observer pattern?</summary>

- It is possible to introduce new subscriber classes without having to change the publisher’s code (Open/Closed Principle);
- It is possible to establish relations between objects at runtime.

</details>

<details>
  <summary>What are cons of a Proxy pattern?</summary>

- Subscribers are notified in random order.

</details>
