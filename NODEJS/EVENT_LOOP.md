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
