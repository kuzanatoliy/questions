# Object-oriented programming

<details>
  <summary>What is an Encapsulation?</summary>

Is hiding information inside a particular namespace (container) to limit direct communication with it. We can have one object/class consisting of different variables and functions. Encapsulation prevents or restricts (e.g., read but not write) interaction with some of them.

</details>

<details>
  <summary>What is an Abstraction?</summary>

The process of generalization (also modeling). We replace a particular thing by its more general model. Allow us not to be coupled with implementation details, to use any implementation, satisfying specific interface.

An abstract class is a class with at least one abstract method. Abstract class's non-abstract methods can have implementations, but a class itself can't.

An interface is an abstract class, which methods are only abstract.

</details>

<details>
  <summary>What is an Inheritance?</summary>

Is an ability of a class/object to take some properties from another class/object. In both classical OOP, and JS we can inherit a whole method. As for fields: in classical OOP, we can only inherit its name and type - in JS, we can inherit a field value in addition.

Types:

- single (superclass -> subclass)
- multilevel (superclass -> subclass -> subsubclass)
- hierarchical (superclass -> (subclass1 subclass2))
- multiple ((superclass1 superclass2) -> subclass)
- hybrid (mix of above)

</details>
