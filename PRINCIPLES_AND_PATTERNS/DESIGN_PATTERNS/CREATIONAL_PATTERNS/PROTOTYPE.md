# Prototype

<details>
  <summary>What is a Prototype?</summary>

A Prototype is a creational design pattern that lets you copy existing objects without making your code dependent on their classes.

Applicability:

- Use the Prototype pattern when there isn't dependency from the concrete classes of copied objects in a code.
- Use the pattern when you want to reduce the number of subclasses that only differ from the initialization of their respective objects. Somebody could have created these subclasses to be able to create a new one with a specific configuration.

Pros:

- Clone objects without coupling to their concrete classes.
- Get rid of repeated initialization code in favour of cloning pre-built prototypes.
- Produce complex exemplars more conveniently.
- Get an alternative to inheritance when dealing with configuration presets.

Cons:

- Cloning complex objects that have circular references might be very tricky.

[More >>](https://refactoring.guru/design-patterns/prototype)

</details>
