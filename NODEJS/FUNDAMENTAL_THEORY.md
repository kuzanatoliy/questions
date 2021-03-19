# Fundamental theory

## Links
[NodeJS Tutorial](https://www.tutorialsteacher.com/nodejs/nodejs-tutorials)

## Node.js introduction. Modules. NPM

### Links
[NodeJS Releases](https://nodejs.org/en/about/releases/)

### Questions

<details>
  <summary>What is NodeJS? How could it be used?</summary>

  NodeJS is a programming platform for running JavaScript and turning the language into a common language. Also, NodeJS adds opportunities to communicate with output/input through NodeJS API and use external modules. The base using sphere is the development of web-servers. Moreover, NodeJS allows creating desktop applications(for example, it is possible to use Electron). NodeJS uses an event-driven model and async or reactive programming with not blocked output/input.
  For using could be downloaded one of the NodeJS versions from the official website. Besides, it is possible to turn between versions with the nvm application.

</details>

<details>
  <summary>How is NodeJS versioning defined?</summary>

  There are two groups of NodeJS versions. First odd-numbered releases (9, 11, etc.), and second even-numbered or LTS releases (10, 12, etc.). LTS releases have long term support which typically guarantees that NodeJS developers will fix critical problems(bugs). As a result, the production application should use only LTS versions. There are follow life cycle periods:
  Not supported - version is not supported anymore;
  Current - version is in active development;
  Active - version is recommended to use;
  Maintenance - version is supported.

</details>

<details>
  <summary>What types of modules are used/supported in NodeJS?</summary>
  
  NodeJS includes three types of modules:
  1. Core Modules
  2. Local Modules
  3. Third-Party Modules
  The core modules include the bare minimum functionalities of NodeJS. Core modules are compiled into their binary distribution and automatically load when NodeJS starts the process. However, it is required to import the core module first to use it in your application.
  Local modules are modules created locally in your Node.js application. These modules include different functionalities of your application in separate files and folders. You can also package it and distribute it via NPM. For example, if it is needed to connect to MongoDB and fetch data, it will be possible to create a reusable module.
  Third-Party Modules are modules that are possible to import from NPM.


</details>

What is NPM and how to use it?
What is package.json, its structure and purpose?
What are NPM scripts and how to use them?
What are package dependencies and what are their main types?

## Events and Event Loop. Async Development Introduction

### Links

### Questions

How does Node.js interact with asynchronous code?
What is Node.js Event Loop?
How does it work?What is EventEmitter and how does event system work in Node.js?
What is a memory leak and what causes it?
How to work with filesystem in Node.js?
What are the main pros and cons of interacting with filesystem synchronously and asynchoronously?
What is a Buffer? How can it be used?
What is a Stream?What are the benefits of using them while interacting with filesystem?
