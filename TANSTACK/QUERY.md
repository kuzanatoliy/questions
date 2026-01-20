# Query

<details>
  <summary>What requirements are for the tanstack(reqct) query library?</summary>

React queries is optimized for modern browsers. It is compatible with the following browsers:

- Chrome >= 91
- Firefox >= 90
- Edge >= 91
- Safari >= 15
- iOS >= 15
- Opera >= 77

[More >>](https://tanstack.com/query/latest/docs/framework/react/installation#requirements)

</details>

<details>
  <summary>What query is?</summary>

A query is a declarative dependency on an asynchronous source of data that is tied to a unique key. A query can be used with any Promise based method.

For example:

    import { useQuery } from '@tanstack/react-query'

    function App() {
      const info = useQuery({ queryKey: ['todos'], queryFn: fetchTodoList })
    }

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/queries)

</details>

<details>
  <summary>What query key is?</summary>

A query key has to be an Array at the top level, and can be as simple as an Array with a single string, or as complex as an array of many strings and nested objects.

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/query-keys)

</details>
