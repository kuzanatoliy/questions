# Logging and error handling

## Logging. Error Handling

### Links
[Debug](https://www.npmjs.com/package/debug)
[Debug-levels](https://www.npmjs.com/package/debug-levels)
[Winston](https://www.npmjs.com/package/winston)
[Bunyan](https://www.npmjs.com/package/bunyan)

### Questions

<details>
  <summary>What are logs?</summary>
  
  Logs are the events that reflect the various aspect of an application. It is the mode of troubleshooting and diagnosing your application if written correctly by the team.

</details>

<details>
  <summary>How to log entities in Node.js?</summary>

  It is possible to use one of the most popular logging libraries as Winston or Debug. It is necessary to configure the logger and import function into the code and call function.

</details>

<details>
  <summary>What are the base levels of logging used in Node.js?</summary>

  In the usual situation, NodeJS application has the following levels:
  Debug - fine-grained informational events that are most useful to debug an application.
  Info - informational messages that highlight the progress of the application at a coarse-grained level.
  Warn - potentially harmful situations.
  Error - error events that might still allow the application to continue running.
  Fatal - very severe error events that will presumably lead the application to abort.

</details>

<details>
  <summary>What are the pros and cons of a debug logger?</summary>

  Debug is a tiny JavaScript debugging utility modelled after Node.js core's debugging technique. Works in Node.js and web browsers.
  Pros:
  + It is a simple solution.
  + A big community.
  + Common solution for NodeJS and browser.
  Cons:
  - This logger doesn't have levels but can be extended by a debug-levels package.
  - The output into an error stream.

</details>

<details>
  <summary>What are the pros and cons of a bunyan logger?</summary>

  Prons:
  + Use JSON format.
  + Has logger levels.
  + Configure output streams.
  + Has CLI.
  + Support runtime environments.

</details>

<details>
  <summary>What are the main error types in Node.js?</summary>

  Applications running in Node.js will generally experience four categories of errors:
  
  * Standard JavaScript errors such as ```<EvalError>```, ```<SyntaxError>```, ```<RangeError>```, ```<ReferenceError>```, ```<TypeError>```, and ```<URIError>```.
  * System errors.
  * Custom application errors.
  * AssertionErrors are a speciality class of errors that can be triggered when Node.js detects an exceptional logic violation that should never occur. These are raised typically by the assert module.
  
  All JavaScript and system errors raised by Node.js inherit from, or are instances of, the standard JavaScript <Error> class and are guaranteed to provide at least the properties available on that class.

</details>

How to setup error handling in Node.js?
What is an uncaught exception in Node.js and how to handle it?

## Command Line. Debugging

### Links

### Questions

How to work with CLI in Node.js?
How to debug Node.js applications?
What are the main approaches and solutions?
How to debug Node.js applications with Chrome DevTools?