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

<details>
  <summary>What objective of allowing users to provide preferences for the display of conforming alternate versions?</summary>

The objective of this technique is to provide a mechanism for users to select a preference for an alternate conforming version of a Web page.

**Procedure:**

1. Change a preference for how pages on the site are displayed.
2. Check that the preference itself or a link to that page where it can be set can be reached from each non-conforming page.
3. Check that Web pages are displayed according to the selected preference.
4. Check that when the preference(s) are set, the Web page confroms as claimed.
5. Verify that the resulting page is a conformaing alternate version for the original page.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/server-side-script/SVR4)

</details>

<details>
  <summary>What objective of specifying the default language in the HTTP header?</summary>

The objective of this technique is to provide information on the primary language or languages in a Web page, in order to identify the audience of the content. The Content-Language HTTP header can contain a list of one or more language codes, which can be used for language negotiation between a user agent and a server. If the language preferences in a user agent are set correctly, language negotiation can help the user to find a language version of the content that suits their preferences.

**Procedure:**

1. Use a Live HTTP Header viewer to find the value of the Content-Language header.
2. Check that this value matches the default language of the Web page.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/server-side-script/SVR5)

</details>
