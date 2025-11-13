# Next

<details>
  <summary>How to improve specify target browser versions?</summary>

The Next allows to specify target browser that can affect bundle sizes for application because of system will use or not transpaling properties depended on browser support. For it need to add `browserlist` property to `package.json` with supported browser list.

**For example:**

    {
    "browserslist": ["chrome 111", "edge 111", "firefox 111", "safari 16.4"]
    }

[More >>](https://nextjs.org/docs/architecture/supported-browsers)

</details>

<details>
  <summary>What is dynamic function in nextjs?</summary>

The next/dynamic is function that should be used for dynamic components to integrate them into system. It should allows to improve application performance. Moreover, could be used in specific corner cases to avoid server side rendering.

[More >>](https://nextjs.org/docs/pages/guides/lazy-loading#with-named-exports)

</details>
