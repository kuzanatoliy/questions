# Template method

<details>
  <summary>What is the Template Method?</summary>

Template Method is a behavioural design pattern that defines the skeleton of an algorithm in the superclass but lets subclasses override specific steps of the algorithm without changing its structure. Also could be useful for the Open-Close principle.

Applicability:

- Use the Template Method pattern when you want to let clients extend only steps of an algorithm, but not the whole algorithm or its structure.
- Use the pattern when you have several classes that contain almost identical algorithms with some minor differences. As a result, you might need to modify all when the algorithm changes.

Prons:

- You can let clients override only certain parts of a large algorithm, making them less affected by changes into other parts of the algorithm.
- You can pull the duplicate code into a superclass.

Cons:

- You might violate the Liskov Substitution Principle by suppressing a default step implementation via a subclass.
  Template methods tend to be harder to maintain the more steps they have.

[More >>](https://refactoring.guru/design-patterns/template-method)

</details>
