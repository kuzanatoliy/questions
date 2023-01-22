# Template method

### Links

[Refactoring guru / template method](https://refactoring.guru/design-patterns/template-method)

<details>
  <summary>What is a Template method?</summary>

Template Method is a behavioral design pattern that defines the skeleton of an algorithm in the superclass but lets subclasses override specific steps of the algorithm without changing its structure.

</details>

<details>
  <summary>What is a Template method's Applicability?</summary>

- Use the Template Method pattern when you want to let clients extend only particular steps of an algorithm, but not the whole algorithm or its structure;
- Use the pattern when you have several classes that contain almost identical algorithms with some minor differences. As a result, you might need to modify all classes when the algorithm changes.

</details>

<details>
  <summary>What are pros of a Template method pattern?</summary>

- It is possible to let clients override only certain parts of a large algorithm, making them less affected by changes that happen to other parts of the algorithm.
- It is possible to pull the duplicate code into a superclass.

</details>

<details>
  <summary>What are cons of a Proxy pattern?</summary>

- Some clients may be limited by the provided skeleton of an algorithm;
- You might violate the Liskov Substitution Principle by suppressing a default step implementation via a subclass;
- Template methods tend to be harder to maintain the more steps they have.

</details>
