# Flyweight

### Links

[Refactoring guru / flyweight](https://refactoring.guru/design-patterns/flyweight)

<details>
  <summary>What is a Flyweight?</summary>

Flyweight is a structural design pattern that lets you fit more objects into the available amount of RAM by sharing common parts of state between multiple objects instead of keeping all of the data in each object.

</details>

<details>
  <summary>What is a Flyweight's Applicability?</summary>

- Use the Flyweight pattern only when your program must support a huge number of objects which barely fit into available RAM.

</details>

<details>
  <summary>What are pros of a Flyweight pattern?</summary>

- It is possible to save lots of RAM, assuming your program has tons of similar objects.

</details>

<details>
  <summary>What are cons of a Flyweight pattern?</summary>

- It’s possible to be trading RAM over CPU cycles when some of the context data needs to be recalculated each time somebody calls a flyweight method;
- The code becomes much more complicated. New team members will always be wondering why the state of an entity was separated in such a way.

</details>
