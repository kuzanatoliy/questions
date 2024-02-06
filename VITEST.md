# vitest

<details>
  <summary>What pools could be used in vitest?</summary>

- **threads** - Enable multi-threading using tinypool (a lightweight fork of Piscina).

- **forks** - Similar as threads pool but uses child_process instead of worker_threads via tinypool.

- **vmThreads** - Run tests using VM context (inside a sandboxed environment) in a threads pool.

- **vmForks** - Similar as vmThreads pool but uses child_process instead of worker_threads via tinypool.

[More >>](https://vitest.dev/config/#pool-1-0-0)

</details>
