# Flyweight

<details>
  <summary>What is Flyweight?</summary>

Flyweight is a structural design pattern that lets you fit more objects into the available amount of RAM by sharing common parts of the state between multiple exemplars instead of keeping all of the data in each object.

Applicability:

- Use the Flyweight pattern only when it is needed to optimize used RAM.

Prons:

- It is possible to save lots of RAM, assuming your program has tons of similar objects.

Cons:

- It is possible to trade RAM over CPU cycles when some context data needs recalculation each time somebody calls a flyweight method.
- The code becomes much more complicated. New team members will always be wondering about the state.

[More >>](https://refactoring.guru/design-patterns/flyweight)

</details>
