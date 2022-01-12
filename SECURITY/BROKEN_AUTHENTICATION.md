# Broken Authntication

## Links
[OWASP: Broken Authentication](https://owasp.org/www-project-top-ten/2017/A2_2017-Broken_Authentication)

## Questions

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
