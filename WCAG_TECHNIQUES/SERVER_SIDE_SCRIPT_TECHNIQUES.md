# Server-Side Script Techniques

<details>
  <summary>What objective of implementing automatic redirects on the server side instead of on the client side?</summary>

The objective of this technique is to avoid confusion that may be caused when two new pages are loaded in quick succession because on page redirects to another. Some user agents supprt the use of the HTML meta element to redirect the user to another page after a specified number of seconds. This makes a page inaccessible to some users, especially users with screen readers. Server-side technologies provide methods to implement redirects in a way that does not confuse users. A server-side script or configuration file can cause the server to send an appropriate HTTP response with a status code in the 3xx range and a Location header with another URL. When the browser recives this response, the location bar changes and the browser makes a request with the new URL.

**Procedure:**

1. Find each link or programmatic reference to another page or Web page.
2. For each link or programmatic reference to a URI in the set of Web pages being evaluated, check if the referenced Web page contains code that causes a client-side redirct.
3. For each link or programmatic reference to a URI in the set of Web pages being evaluated, check if the referenced URI does not cause a redirect OR causes a server-side redirect without a time-out.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/server-side-script/SVR1)

</details>
