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
