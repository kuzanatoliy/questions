# Strategy

<details>
  <summary>What is Strategy?</summary>

Strategy is a behavioural design pattern that lets you define a family of algorithms, but each of them into a separate class, and make their objects interchangeable. The pattern could be useful for Open-Close principle because allows to add new functionality by new strategy.

Applicability:

- Use the Strategy pattern when you want to use different variants of an algorithm within an object and switch from one algorithm to another during runtime.
- Use the Strategy when you have a lot of similar classes that only differ in executing some behaviour.
- Use the pattern to isolate the business logic from the implementation details of algorithms that may not be as important.
- Use it when your class has a massive conditional operator that switches between different variants of the same algorithm.

Prons:

- You can swap algorithms used inside an object at runtime.
- You can isolate the implementation details of an algorithm from the code that uses it.
- You can replace inheritance with composition.
- Open/Closed Principle. You can introduce new strategies without having to change the context.

Cons:

- If you only have a couple of algorithms and they rarely change, there is no real reason to overcomplicate the program with new classes and interfaces that come along with the pattern.
- Clients must be aware of the differences between strategies to be able to select a proper one.
- Many modern programming languages have functional type support that lets you implement different versions of an algorithm inside a set of anonymous functions.

[More >>](https://refactoring.guru/design-patterns/strategy)

</details>
