# Singleton

<details>
  <summary>What is Singleton?</summary>

Singleton is a creational design pattern that guarantee that a class or an entity has only one instance and provide global access point.

</details>

<details>
  <summary>What is Singleton?</summary>

Singleton is a creational design pattern that lets you ensure that a class has only one instance while providing a global access point to this instance.

Applicability:

- Use the Singleton pattern when a class in your program should have just a single instance available to all clients; for example, a single database object shared by different parts of the program.
- Use the Singleton pattern when you need stricter control over global variables.

Pros:

- You can be sure that a class has only a single instance.
- You gain a global access point to that instance.
- The initialization of the singleton object happens during the first call.

Cons:

- Single Responsibility Principle. The pattern solves two problems at the time.
- The Singleton pattern can mask unluck design, for instance, when the program components know too much about each other.
- The pattern requires special treatment in a multithreaded environment so that multiple threads cannot create a singleton object several times.
- It may be difficult to unit test the client code because many test frameworks rely on inheritance when producing mock objects. Since the constructor of the singleton class is private and overriding static methods is impossible in most languages, you will need to think of a creative way to mock the singleton.

[More >>](https://refactoring.guru/design-patterns/singleton)

</details>
