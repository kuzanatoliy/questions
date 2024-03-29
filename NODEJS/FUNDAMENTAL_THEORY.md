# Fundamental theory

### Links

[NodeJS Tutorial](https://www.tutorialsteacher.com/nodejs/nodejs-tutorials)

## Node.js introduction. Modules. NPM

### Links

[NodeJS Releases](https://nodejs.org/en/about/releases/)
[NPM docs](https://docs.npmjs.com/about-npm)

### Questions

<details>
  <summary>What is NodeJS? How could it be used?</summary>

NodeJS is a programming platform for running JavaScript and turning the language into a common language. Also, NodeJS adds opportunities to communicate with output/input through NodeJS API and use external modules. The base using sphere is the development of web-servers. Moreover, NodeJS allows creating desktop applications(for example, it is possible to use Electron). NodeJS uses an event-driven model and async or reactive programming with not blocked output/input.

For using, one of the NodeJS versions could be downloaded from the official website. Besides, it is possible to turn between versions with the nvm application.

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

<details>
  <summary>What is NPM? How to use it?</summary>

Node Package Manager (NPM) is a command-line tool that installs, updates or uninstalls Node.js packages in your application. It is also an online repository for open-source Node.js packages. The node community around the world creates modules and publishes them as packages in this repository. Npm allows installing, uninstalling and updating packages.

</details>

<details>
  <summary>What is package.json, its structure and purpose?</summary>

Package.json file contains information about an application: name, version, dependencies, and etc. Each directory in the file is interpreted as a NodeJS package.

</details>

<details>
  <summary>What are NPM scripts? How to use them?</summary>
  
  The scripts property of a package.json file contains scripts that can be run by ```npm run <stage>```. Also, It is possible to use pre and post commands as prepare, prepublish, prepublishOnly and .etc.

</details>

<details>
  <summary>What are package dependencies? What are their main types?</summary>
  
  Dependencies are a list of external modules that a project uses.

NodeJS contains two dependency types:

1. Dependencies should have dependencies that the production mode will use.
2. devDependencies should have dependencies that will be used in development. For example, linter, bable and etc.

</details>

## Events and Event Loop. Async Development Introduction

### Links

[Event](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/)
[Events](https://nodejs.org/api/events.html)

### Questions

<details>
  <summary>What is EventEmitter? How does the event system work in NodeJS?</summary>

All objects that emit events are instances of the EventEmitter class. These objects expose an `eventEmitter.on()` function that allows one or more functions to be attached to named events emitted by the object. Typically, event names are camel-cased strings but any valid JavaScript property key can be used.

When the EventEmitter object emits an event, all of the functions attached to that specific event are called synchronously. Any values returned by the called listeners are ignored and discarded.

The following example shows a simple EventEmitter instance with a single listener. The `eventEmitter.on()` method is used to register listeners, while the `eventEmitter.emit()` method is used to trigger the event.

</details>
