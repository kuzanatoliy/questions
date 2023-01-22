# Strategy

### Links

[Refactoring guru / strategy](https://refactoring.guru/design-patterns/strategy)

<details>
  <summary>What is a Strategy?</summary>

Strategy is a behavioral design pattern that lets you define a family of algorithms, put each of them into a separate class, and make their objects interchangeable.

</details>

<details>
  <summary>What is a Strategy's Applicability?</summary>

- Use the Strategy pattern when you want to use different variants of an algorithm within an object and be able to switch from one algorithm to another during runtime;
- Use the Strategy when you have a lot of similar classes that only differ in the way they execute some behavior;
- Use the pattern to isolate the business logic of a class from the implementation details of algorithms that may not be as important in the context of that logic;
- Use the pattern when your class has a massive conditional statement that switches between different variants of the same algorithm.

</details>

<details>
  <summary>What are pros of a Strategy pattern?</summary>

- It is possible to swap algorithms used inside an object at runtime;
- It is possible to isolate the implementation details of an algorithm from the code that uses it;
- It is possible to replace inheritance with composition;
- It is possible to introduce new strategies without having to change the context (Open/Closed Principle).

</details>

<details>
  <summary>What are cons of a Proxy pattern?</summary>

- If you only have a couple of algorithms and they rarely change, there’s no real reason to overcomplicate the program with new classes and interfaces that come along with the pattern;
- Clients must be aware of the differences between strategies to be able to select a proper one;
- A lot of modern programming languages have functional type support that lets you implement different versions of an algorithm inside a set of anonymous functions. Then you could use these functions exactly as you’d have used the strategy objects, but without bloating your code with extra classes and interfaces.

</details>
