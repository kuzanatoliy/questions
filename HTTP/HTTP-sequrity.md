# HTTP sequrity

<details>
  <summary>What is content sequrity policy (CSP)?</summary>

Content Security Policy (CSP) is an added layer of security that helps to detect and mitigate certain types of attacks, including Cross-Site Scripting (XSS) and data injection attacks. These attacks are used for everything from data theft, to site defacement, to malware distribution?

[More >>](https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP#threats)

</details>

<details>
  <summary>What difference between Content-Security-Policy and Content-Security-Policy-Report-Only?</summary>

The Content-Security-Policy-Report-Only creates and sends report about attemts of an unexpected comunication.
The Content-Security-Policy prevents the unexpected requests.
These policies could be used together and if they were in one response both of them would be honored.

</details>

<details>
  <summary>What is Certificate Transparency?</summary>

Certificate Transparency is an open framework designed to protect against and monitor for certificate mis-issuances. It's defined in [RFC 9162](https://www.rfc-editor.org/rfc/rfc9162). With certificate transparency, newly-issued certificates are 'logged' to publicly-run, often independent CT logs — which maintain an append-only, cryptographically-assured record of issued TLS certificates.

</details>

<details>
  <summary>What is Strict transport security?</summary>

The HTTP Strict-Transport-Security response header (often abbreviated as HSTS) informs browsers that the site should only be accessed using HTTPS, and that any future attempts to access it using HTTP should automatically be converted to HTTPS.

Example:

    Strict-Transport-Security: max-age=63072000; includeSubDomains; preload

[More >>](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Strict-Transport-Security)

</details>

<details>
  <summary>What is X-Content-Type-Options?</summary>

The X-Content-Type-Options response HTTP header is a marker used by the server to indicate that the MIME types advertised in the Content-Type headers should be followed and not be changed.

[More >>](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Content-Type-Options)

</details>

<details>
  <summary>What is X-Frame-Options?</summary>

The X-Frame-Options HTTP response header can be used to indicate whether or not a browser should be allowed to render a page in a frame, iframe, embed or object. Sites can use this to avoid click-jacking attacks, by ensuring that their content is not embedded into other sites.

[More >>](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options)

Examples:

    X-Frame-Options: DENY
    X-Frame-Options: SAMEORIGIN

</details>
