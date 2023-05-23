# Functional programming

<details>
  <summary>What characteristics of a Pure function?</summary>

**Idempotence** is a property of an expression to have the same output with an equal input. This term is applicable, e.g., to functions or REST API methods. Notice, that idempotent function still can have side effects.

**Side effects** are any effects produced during an execution of some function/method which is not reflected in its output and usually not its direct goal. Examples: modifying a value of a global variable, any other I/O (screen, file, etc.), calling other side effect functions.

**Pure functions** are idempotent functions without side effects. The purity simplifies a testing process, allows chaining of function calls, allows cashing because of referential transparency.

**Referential transparency** is a property of an expression to stay the same after replacing it with its corresponding value (and vice-versa). Pure functions are always referentially transparent, and we can easily replace them with their output.

</details>
