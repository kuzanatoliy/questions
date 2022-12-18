# Proxy

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
