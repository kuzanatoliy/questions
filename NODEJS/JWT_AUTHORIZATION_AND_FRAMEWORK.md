# JWT authorization and framework

## Authorization. Security. CORS

### Links
[Authentication vs authorization](https://medium.datadriveninvestor.com/authentication-vs-authorization-716fea914d55)
[Passport docs](http://www.passportjs.org/docs/)
[JWT](https://jwt.io/introduction)
[Ten top security risks](https://owasp.org/www-project-top-ten/)

### Questions

<details>
  <summary>What are the differences between authentication and authorization?</summary>
  
  A lot of times, authentication and authorization are mixed sentences. But they have differences between each other.

  Authentication is validating user credentials such as username, password, etc. An authenticating system usually identities users by a username and password. Besides, the auth systems could have different elements. Based on the security level, authentication factors can vary from one of the following:
  
  * Single-Factor Authentication: This is the simplest form of authentication method, which requires a password to grant user access to a particular system such as a website or a network. 
  
  * Two-Factor Authentication: This is the most popular and safe authentication type. It requires not only a username and password but also a piece of information only the user knows. 
  
  * Multi-Factor Authentication: This is the most advanced type of authentication, which requires two or more levels of security from independent categories of authentication to grant user access to the system.
  
  Authorization is a process that allows getting access to resources such as files, databases, APIs, etc. So authorization verifies user rights.

</details>

<details>
  <summary>How to set up authentication in the NodeJS service using Passport.js?</summary>
  
  Passport is authentication middleware for Node.js. Extremely flexible and modular. Any application based on express.js can use it. A comprehensive set of strategies support authentication using a username and password, Facebook, Twitter, and more.
  
  So for using, it is possible to install Passport.js and one or more strategies. For more look into documentation.

</details>

<details>
  <summary>What is a JSON Web Token?</summary>
  
  JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

</details>

<details>
  <summary>When should you use JSON Web Tokens?</summary>
  
  It is possible to use JWT for authorization and information exchange:

  * Authorization: It is the most common scenario for using JWT. After the login process, each request will include the JWT, which allows getting access.
  
  * Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed - for example, using public/private key pairs - you can be sure the senders are who they say they are.

</details>

<details>
  <summary>What is the JSON Web Token structure?</summary>
  
  JWT contains three parts:

  * Header. Generally, it has two values: type of the token (JWT), and the signing algorithm, such as HMAC SHA256 or RSA.
  
  * Payload. The part of the token, which contains the claims. There are three types of claims: registered, public, and private.
  
  * Signature. It allows verifying that the message wasn't changed.

</details>

<details>
  <summary>How do JSON web Tokens work?</summary>

  In authentication, when the user successfully logs in using their credentials, the server returns JWT. In general, you should not keep tokens longer than required.

  Whenever the user wants to access a protected route or resource, the user agent should send the JWT, typically in the Authorization header using the Bearer schema.

</details>

<details>
  <summary>What is injection risk?</summary>

  The injection flaws, such as SQL, NoSQL, OS, and LDAP injection, occur when an application includes untrusted data as part of a command or query. So attackers can trick and run some commands without proper authorization. So, the application can lose, change data or disclose them to unauthorized parties. From time to time, it is possible to lose control of a host.

  The application is vulnerable to attack when:

  * User-supplied data is not validated, filtered, or sanitized by the application.
  The application uses dynamic queries or non-parameterized calls without context-aware escaping.

  * Hostile data are used within object-relational mapping (ORM) search parameters to extract additional, sensitive records.

  * Dangerous data are used or concatenated, such that the SQL or command contains both structure and hostile data in dynamic queries or stored procedures.

  Solving:

  * The preferred option is to use a safe API, which avoids using the interpreter entirely or provides a parameterized interface or migrate to use Object Relational Mapping Tools (ORMs).

  * Use positive or whitelist server-side input validation. It is not a complete defence as many applications require special characters, such as text areas or APIs for mobile applications.

  * For any residual dynamic queries, escape special characters.

  * Use LIMIT and other SQL controls within queries to prevent mass disclosure of records in case of SQL injection.

  Example:
  
  An application uses untrusted data in the construction of the following vulnerable SQL call:
  
  ```String query = "SELECT * FROM accounts WHERE custID='" + request.getParameter("id") + "'";```

  In both cases, the attacker modifies the id parameter value in their browser to send: ```' or '1'='1```. For example:

  ```http://example.com/app/accountView?id=' or '1'='1```

</details>

<details>
  <summary>What is broken authentication risk?</summary>

  Application authentication and session management functionality often have an implementation that allows attackers to compromise passwords, keys, session tokens, etc.

  Confirmation of the user identity, authentication, and session management is critical to protect against authentication-related attacks. There may be authentication weaknesses if the application:

  * Permit automated attacks such as credential stuffing, where the attacker has a list of valid usernames and passwords.

  * Permit brute force or other automated attacks.

  * Permit default, weak, or well-known passwords, such as Password1 or admin/admin.

  * Use weak or ineffective credential recovery and forget password processes, such as knowledge-based answers, which cannot be made safe.

  * Uses plain text, encrypted, or weakly hashed passwords (see A3:2017-Sensitive Data Exposure).

  * Have missing or ineffective multi-factor authentication.

  * Exposes Session IDs in the URL (e.g., URL rewriting).

  * Do not rotate Session IDs after successful login.

  * Do not invalidate Session IDs. User sessions or authentication tokens.

  Solving:

  * Where possible, implement multi-factor authentication to prevent credential stuffing, brute force, and stolen credential reuse attacks.

  * Do not ship or deploy with any default credentials, particularly for admin users.

  * Implement weak password checks, such as testing new or changed passwords against a list of the top 10000 worst passwords.

  * Align password length, complexity and rotation policies.

  * Ensure registration, credential recovery, and API pathways have protection against account enumeration attacks by using the same messages for all outcomes.

  * Limit or increasingly delay failed login attempts. Log all failures and alert administrators when credential stuffing, brute force, or other attacks are detected.

  * Use a server-side, secure, built-in session manager that generates a new random session ID with high entropy after login. Session IDs should not be in the URL, be securely stored and invalidated after logout, idle, and absolute timeouts.

</details>

<details>
  <summary>What is sensitive data exposure?</summary>

  Many web applications and APIs do not protect sensitive data, such as financial, healthcare, and PII. Attackers may steal or modify such weakly protected data to conduct credit card fraud, identity theft, or other crimes. Sensitive data may be compromised without extra protection, such as encryption at rest or in transit, and requires special precautions when exchanged with the browser.

  The first thing is to determine the protection needs of data in transit and at rest. For example, passwords, credit card numbers, health records, personal information and business secrets require extra protection. For all such data:

  * Protocols such as HTTP, SMTP and FTP should be concerned because they transmit data into clear text.

  * Using old or weak cryptographic algorithms.

  * Using weak crypto keys.

  * Using not enforced encryption.

  * Using invalid certificates.

  Do the following, at a minimum, and consult the references:

  * Classify data processed, stored or transmitted by an application. Identify which data is sensitive according to privacy laws, regulatory requirements, or business needs.

  * Apply controls as per the classification.

  * Avoid storing sensitive data unnecessarily. Discard it as soon as possible or use PCI DSS compliant tokenization or even truncation. 

  * Make sure to encrypt all sensitive data at rest.

  * Ensure up-to-date and more secure standard algorithms, protocols, and keys are in place; use proper key management.

  * Encrypt all data in transit with security protocols such as TLS with perfect forward secrecy (PFS) cyphers.

  * Disable caching for a response that contains sensitive data.

  * Store passwords using adaptive and salted hashing functions with a work factor (delay factor).

  * Verification.

</details>