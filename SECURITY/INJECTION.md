# Injection

## Links
[OWASP: injection](https://owasp.org/www-project-top-ten/2017/A1_2017-Injection)

## Questions

<details>
  <summary>What is the injection?</summary>

  It is possible to inject data into almost all sources. Injection flaws occur when an attacker can send hostile data. Injection vulnerabilities are very prevalent, particularly in legacy code. SQL, LDAP, XPath or NoSQL queries, OS commands, XML parsers, SMTP headers, expression languages and ORM queries often are vulnerable to injection. The injection can result in data loss, corruption, disclosure to unauthorized parties, loss of accountability, or denial of access. Also, the injection can sometimes lead to a complete host takeover.

</details>

<details>
  <summary>When is an application is vulnerable?</summary>

  * when user-supplied data is not validated, filtered, or sanitized by the application;

  * when dynamic queries or non-parameterized calls without context-aware escaping are used directly in the interpreter;

  * when using hostile data within object-relational mapping (ORM) search parameters to extract additional, sensitive records;

  * when the SQL or command contains both structure and hostile data in dynamic queries, commands, or stored procedures (directly using).

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
