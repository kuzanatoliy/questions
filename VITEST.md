# vitest

<details>
  <summary>What pools could be used in vitest?</summary>

- **threads** - Enable multi-threading using tinypool (a lightweight fork of Piscina).

- **forks** - Similar as threads pool but uses child_process instead of worker_threads via tinypool.

- **vmThreads** - Run tests using VM context (inside a sandboxed environment) in a threads pool.

- **vmForks** - Similar as vmThreads pool but uses child_process instead of worker_threads via tinypool.

[More >>](https://vitest.dev/config/#pool-1-0-0)

</details>

<details>
  <summary>What settings would be used for the threads pool?</summary>

- **maxThreads** - Maximum number of threads. You can also use `VITEST_MAX_THREADS` environment variable.

- **minThreads** - Minimum number of threads. You can also use `VITEST_MIN_THREADS` environment variable.

- **singleThread** - Run all tests with the same environment inside a single worker thread. This will disable built-in module isolation (your source code or inlined code will still be reevaluated for each test), but can improve test performance.

- **useAtomics** - Use Atomics to synchronize threads.

- **isolate** - Isolate environment for each test file.

- **execArgv** - Pass additional arguments to `node` in the threads.

[More >>](https://vitest.dev/config/#pooloptions-threads)

</details>

<details>
  <summary>What settings would be used for the forks pool?</summary>

- **maxForks** - Maximum number of forks.

- **minForks** - Minimum number of forks.

- **singleFork** - Run all tests with the same environment inside a single child process.

- **isolate** - Isolate environment for each test file.

- **execArgv** - Pass additional arguments to `node` in the child processes.

[More >>](https://vitest.dev/config/#pooloptions-forks)

</details>
