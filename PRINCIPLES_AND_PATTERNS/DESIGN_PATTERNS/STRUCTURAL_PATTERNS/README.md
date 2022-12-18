# Structural patterns

<details>
  <summary>What is Adapter?</summary>

The adapter is a structural design pattern that allows objects with incompatible interfaces to collaborate.

Applicability:

- Use the adapter when you want to use some existing class, but its interface is not compatible with the rest of your code.
- Use the pattern for reusing several existing subclasses that lack some functionality, and there is not possible to add it in the superclass.

Prons:

- Single Responsibility Principle. You can separate the interface or data conversion code from the primary business logic of the program.
- Open/Closed Principle. You can introduce new types of adapters into the program without breaking the existing client code, as long as they work with the adapters through the client interface.

Cons:

- The overall complexity of the code increases because it requires introducing a set of new interfaces and classes. From time to time, changing into service is an easier way.

[More >>](https://refactoring.guru/design-patterns/adapter)

</details>

<details>
  <summary>What is Bridge?</summary>

The Bridge is a structural design pattern that lets you split a large class or a set of closely related classes into two separate hierarchies - abstraction and implementation - their implementation independent of each other.

Applicability:

- Use the Bridge pattern when you want to divide and organize a class with several functional variants (for example, if the implemented class can work with various database servers).
- Use the pattern when you need to extend a class in several orthogonal (independent) dimensions.
- Use the Bridge if you need to be able to switch implementations at runtime.

Prons:

- You can create platform-independent classes and apps.
- The client code works with high-level abstractions.
- Open/Closed Principle. You can introduce new abstractions and implementations independently from each other.
- Single Responsibility Principle. You can focus on high-level logic in the abstraction and on platform details in the implementation.

Cons:

- You might make the code more complicated by applying the pattern to a highly cohesive class.

[More >>](https://refactoring.guru/design-patterns/bridge)

</details>

<details>
  <summary>What is Composite?</summary>

Composite is a structural design pattern that lets you compose objects into tree structures and then work with these structures as if they were individual objects.

Applicability:

- Use the Composite pattern when you have to implement a tree-like object structure.
- Use it when you want the client code to treat both simple and complex elements uniformly.

Prons:

- It is possible to work with complex tree structures more conveniently: use polymorphism and recursion to your advantage.
- Open/Closed Principle. You can introduce new element types into the app without breaking the existing code, which now works with the object tree.

Cons:

- It is difficult to provide a shared interface for classes whose functionality differs too much. In base scenarios, there is possible to overgeneralize the component interface, making it harder to comprehend.

[More >>](https://refactoring.guru/design-patterns/composite)

</details>

<details>
  <summary>What is a Decorator?</summary>

The decorator is a structural design pattern that lets you attach new behaviours to objects by placing these objects inside specialized wrapper objects that contain the behaviours.

Applicability:

- Use the Decorator pattern when it is possible to increase behaviours at runtime without breaking the code that uses these objects.
- Use it when it is impossible to extend behaviour using inheritance.

Prons:

- It is possible to extend a behaviour without making a new subclass.
- It is possible to add or remove responsibilities from an object at runtime.
- It is possible to combine several behaviours by wrapping an object into multiple decorators.
- Single Responsibility Principle. You can divide a monolithic class that implements many possible variants of behaviour into several smaller ones.

Cons:

- It is hard to remove a specific wrapper from the wrappers stack.
- It is hard to implement a decorator with independent behaviour from the stack.
- The initial configuration code of layers might look pretty ugly.

[More >>](https://refactoring.guru/design-patterns/decorator)

</details>

<details>
  <summary>What is a Facade?</summary>

It is a structural design pattern that provides a simplified interface to a library, a framework, or any other complex set of classes.

Applicability:

- Use the Facade pattern when you need to have a limited but straightforward interface to a complex subsystem.
- Use the Facade when you want to structure a subsystem into layers.

Prons:

- It is possible to isolate your code from the complexity of a subsystem.
  Cons:
- A facade can become a god object coupled to all classes of an app.

[More >>](https://refactoring.guru/design-patterns/facade)

</details>

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

<details>
  <summary>What is Proxy?</summary>

Proxy is a structural design pattern that provides a substitute or placeholder for another object. A proxy controls access to the original one, allowing it to perform something either before or after the request gets through to the original one.

Applicability:

- Lazy initialization.
- Access control (protection proxy).
- Logging requests (logging proxy).
- Caching request results (caching proxy).
- Smart reference.

Prons:

- It is possible to control the service object without clients knowing about it.
- It is possible to manage the lifecycle of the service object when clients do not care about it.
- The proxy works even if the service object is not ready or is not available.
- Open/Closed Principle. You can introduce new proxies without changing the service or clients.

Cons:

- The code may become more complicated since you need to introduce a lot of new classes.

[More >>](https://refactoring.guru/design-patterns/proxy)

</details>
