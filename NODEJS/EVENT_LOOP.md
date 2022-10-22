# Event loop

### Links

[The Node.js Event Loop, Timers, and process.nextTick()](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/)

<details>
  <summary>What is the event loop?</summary>

The event loop is what allows Node.js to perform non-blocking I/O operations — despite the fact that JavaScript is single-threaded — by offloading operations to the system kernel whenever possible.

Since most modern kernels are multi-threaded, they can handle multiple operations executing in the background. When one of these operations completes, the kernel tells Node.js so that the appropriate callback may be added to the poll queue to eventually be executed.

</details>

<details>
  <summary>What event loop phases are in nodeJS?</summary>

- **timers**: this phase executes callbacks scheduled by setTimeout() and setInterval().
- **pending callbacks**: executes I/O callbacks deferred to the next loop iteration.
  idle, prepare: only used internally.
- **poll**: retrieve new I/O events; execute I/O related callbacks (almost all with the exception of close callbacks, the ones scheduled by timers, and setImmediate()); node will block here when appropriate.
- **check**: setImmediate() callbacks are invoked here.
- **close callbacks**: some close callbacks, e.g. socket.on('close', ...).

</details>

<details>
  <summary>What timer phase is?</summary>

A timer specifies the threshold after which a provided callback may be executed rather than the exact time a person wants it to be executed. Timers callbacks will run as early as they can be scheduled after the specified amount of time has passed; however, Operating System scheduling or the running of other callbacks may delay them.

[More >>](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/#timers)

</details>

<details>
  <summary>What pending callbacks phase is?</summary>

This phase executes callbacks for some system operations such as types of TCP errors. For example if a TCP socket receives ECONNREFUSED when attempting to connect, some \*nix systems want to wait to report the error. This will be queued to execute in the pending callbacks phase.

[More >>](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/#pending-callbacks)

</details>

<details>
  <summary>What pool phase is?</summary>

The poll phase has two main functions:

1. Calculating how long it should block and poll for I/O, then.
2. Processing events in the poll queue.

[More >>](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/#poll)

</details>

<details>
  <summary>What check phase is?</summary>

This phase allows a person to execute callbacks immediately after the poll phase has completed. If the poll phase becomes idle and scripts have been queued with setImmediate(), the event loop may continue to the check phase rather than waiting.

[More >>](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/#check)

</details>

<details>
  <summary>What close callbacks phase is?</summary>

If a socket or handle is closed abruptly (e.g. socket.destroy()), the 'close' event will be emitted in this phase. Otherwise it will be emitted via process.nextTick().

[More >>](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/#close-callbacks)

</details>

<details>
  <summary>Why use process.nextTick()?</summary>

There are two main reasons:

1. Allow users to handle errors, cleanup any then unneeded resources, or perhaps try the request again before the event loop continues.
2. At times it's necessary to allow a callback to run after the call stack has unwound but before the event loop continues.

</details>
