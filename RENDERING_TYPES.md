# Rendering types

### Links

[Frontend rendering: SSG vs SSR vs CSR vs ISR](https://dexlock.com/blog/frontend-rendering-ssg-vs-ssr-vs-csr-vs-isr/)

### Questions

<details>
  <summary>What types of rendering exist?</summary>

**SSG (Static Site Generation)** - It will run a special function to fetch data once when the page builds.

**SSR (Server Side Rendering)** – It will run a special function to fetch data from API on every page request from the server-side (before the page is loaded, that special function will run first, creating a delay. Only after that, it will serve the page).

**CSR (Client Side Rendering)** - This is the most usual type of data fetching using useEffect. It will fetch the data from the API on every single page request from the client-side (after the page is rendered, the function will run).

**ISR (Incremental Static Regeneration)** - It is a combination of SSG and SSR, where it is served statically, but at a certain time and with a certain condition that page will rebuild and fetch the info from the API again.

</details>
