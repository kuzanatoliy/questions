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

<details>
  <summary>What objective of using .htaccess to ensure that the only way to access non-conforming content is from conforming content?</summary>

The objective of this technique is to ensure that users can always acess an accessible version of the content when non-conforming versions are also available. Whenever content is provided in a format that does not conform to WCAG, the site as a whole can still conform if alternate versions of the inaccessible content are provided. Conformatnce Requirement 4 requires that alternate versions can be derived from the nonconforming content or from its URI.

**Procedure:**

1. Identify pages that do not conform to WCAG at the conformance Level claimed where accessible alternatives are served based on the use of .htaccess files.
2. Visit the URI of the non-conforming content.
3. Verify that the resulting page is one of the following:

- a conforming alternate version for the non-conforming content.
- a page that includes a link to both the conforming alternate version and the non-conforming content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/server-side-script/SVR2)

</details>

<details>
  <summary>What objective of using HTTP referer to ensure that the only way to access non-conforming content is fro mconforming content?</summary>

The objective of this technique is to ensure that users can obtain an accessible version of content where both non-conformgin and conforming versions are provided.

**Procedure:**

1. Identify pages that do not conform to WCAG at the conformance Level claimed where accessible alternatives are served based on HTTP Referrer.
2. Visit the URI of the non-conforming content.
3. Verify that the resulting page is one of the following:

- a conforming alternate version for the non-conforming content.
- a page that includes a link to both the conforming alternate version and the non-conforming content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/server-side-script/SVR3)

</details>
