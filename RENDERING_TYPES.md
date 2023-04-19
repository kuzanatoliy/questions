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

<details>
  <summary>What are pros and cons of SSG?</summary>

**Pros:**

- Static sites are the fastest form of web pages as they are pre-rendered and ready to be served;
- Have great SEO because they pre-render the fetched content;
- Rendering happens at build time on the server, the result is then cached in CDN’s, thus improving the performance as rendering happens once and the result is stored closer to users (solving latency issues).

**Cons:**

- Low Data Integrity as it is only fetched during build time;
- Problematic for sites with many pages due to slow build time;
- The site to be rebuilt, tested and deployed on content updation;
- If content changes frequently, it may become stale as rendering happens only once. Hence, there is a need to trigger a rebuild inorder to update the content.

</details>

<details>
  <summary>What are pros and cons of SSR?</summary>

**Pros:**

- Quick Initial Access: the pages are immediately available to interact with for your users, even on slow Internet connections;
- High Data Integrity, as it fetches on every render;
- Have great SEO because they pre-render the fetched content;
- Great for static sites.

**Cons:**

- If the pages have heavy/complex data, browsing from page to page is slower as here the app is rendered twice, once on the server and then on the client;
- Complex caching;
- Requires a bigger and more powerful server to provide high-performance;
- High Latency: SSR sites tend to slow down in case of heavy traffic.

</details>
