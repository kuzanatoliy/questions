# Query

<details>
  <summary>What are requirements for the tanstack(reqct) query library?</summary>

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
  <summary>What is a query?</summary>

A query is a declarative dependency on an asynchronous source of data that is tied to a unique key. A query can be used with any Promise based method.

For example:

    import { useQuery } from '@tanstack/react-query'

    function App() {
      const info = useQuery({ queryKey: ['todos'], queryFn: fetchTodoList })
    }

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/queries)

</details>

<details>
  <summary>What is a query key?</summary>

A query key has to be an Array at the top level, and can be as simple as an Array with a single string, or as complex as an array of many strings and nested objects.

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/query-keys)

</details>

<details>
  <summary>What is a query function?</summary>

A query function can be literally any function that returns a promise. The promise that is returned should either resolve the data or throw an error.

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/query-functions)

</details>

<details>
  <summary>What is a query options?</summary>

A query options is a helper that returns what you pass but can be useful for type defention.

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/query-options)

</details>

<details>
  <summary>What is a network mode?</summary>

A network mode is an option that control queries and mutations behaviour when application doesn't have network connection. It is possible to use following modes:

- **online** (default mode) - In the mode, queries nad mutations will not fire unless you have network connection. It is possible to recongnize that query / mutation is paused by fetchStatus or isPaused flag.
- **always** - In this mode, queries will always fetch and ignore onlin / offline state, as a result, the queries won't be in pause state.
- **offlineFirst** - The mode is the middle ground between the previous two, where queries will run once, but then can be paused.

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/network-mode)

</details>

<details>
  <summary>What are parallel queries?</summary>

The library allows to run parallel queries by useQueries hook. For example:

    const userQueries = useQueries({
      queries: users.map((user) => {
        return {
          queryKey: ['user', user.id],
          queryFn: () => fetchUserById(user.id),
        }
      }),
    })

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/parallel-queries)

</details>

<details>
  <summary>What are dependent queries?</summary>

Dependent queries depend on previous ones to finish before they can execute. To achive this:

- For useQuery, it is possible to use enabled option.
- For useQueries, it is possible to pass empty array.

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/dependent-queries)

</details>

<details>
  <summary>What are fetching indicators?</summary>

It is possible to use status and isFetching indicator for query or mutation and, even, get global fetching status by `useIsFetchig` hook.

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/background-fetching-indicators)

</details>

<details>
  <summary>What is window focus refetching?</summary>

By default library refresh data in the background and to avoid extra requests it is possible to use `refetchOnWindowFocus` option. When it is set up as true it the system will refetch data when web application will start to be used again.

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/window-focus-refetching)

</details>

<details>
  <summary>How works query retries?</summary>

When a `useQuery` query fails the system will automatically retry the query if that query's request has not reached the max number of consecutive reties (3 by default).

**Options:**

- `retry` - control count of retry requests. It can get boolean value, number and function.
- `retryDelay` - control time between requests.
- `refetchIntervalInBackground` - stop refetching on background.
- `refetchInterval` - allows to have special delay for background refetching.

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/query-retries)

</details>

<details>
  <summary>How works paginated queries?</summary>

The rendering paginated data works by including the page information in the query key. For example:

    const result = useQuery({
      queryKey: ['projects', page],
      queryFn: () => fetchProjects(page),
    })

To optimize user experience it is possible to use `keepPreviousDta` function to demonstrate previous data to demonstrate previous data while the new set of data is loading.

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/paginated-queries)

</details>

<details>
  <summary>How works infinite queries?</summary>

`useInfiniteQuery` is a version of `useQuery` that provides the comfortable interface to work with 'load more' of 'infinite scroll' pattern

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/infinite-queries)

</details>

<details>
  <summary>What is an initial query data?</summary>

The queries allow to pass initial data as `useQuery` option to set up initial query state (It also allows to pass function that will initialize data or get them from cache).

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/initial-query-data)

</details>

<details>
  <summary>What is placeholder data?</summary>

The option is similar as `initialData`, but the data is not persisted to the cache. This comes in handy for situations where you have enough partial or face data to render the query successfully while the actual data is fetched in the background.

[More >>](https://tanstack.com/query/latest/docs/framework/react/guides/placeholder-query-data)

</details>
