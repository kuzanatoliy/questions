# Injection

## Links
[OWASP: injection](https://owasp.org/www-project-top-ten/2017/A1_2017-Injection)

[SAST](https://owasp.org/www-community/Source_Code_Analysis_Tools)

[DAST](https://owasp.org/www-community/Vulnerability_Scanning_Tools)

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
  <summary>How to prevent injection?</summary>

  * Use a safe API, which avoids direct using an interpreter entity or provides a parameterized interface or uses Object Relational Mapping Tools (ORMs);

  * Use a positive serverside input validation;

  * Escape special characters for dynamic queries; 

  * Use LIMIT and other SQL controls within queries to prevent mass disclosure of records in case of SQL injection.

</details>

<details>
  <summary>What tools could help to avoid injection?</summary>

  * Static Application Security Testing (SAST)
  
  * Dynamic Application Security Testing (DAST)

</details>

<details>
  <summary>What are the criteria for secure database access?</summary>

  * secure queries:

  SQL Injection occurs when untrusted user input is dynamically added to a SQL query in an insecure manner, often via basic string concatenation. An attacker can get a foothold on your network by it. The best way of protection is using a programming technique known as query Parameterization. It allows the database to distinguish between code and data.

  * secure configuration:

  It is possible to use a secure database configuration. Need to be sure that security controls are available from the Database Management System and hosting platform is enabled and properly configured.

  * secure authentication:

  Authentication should take place only over a secure channel.

  * secure communication:

  Most DBMS support a set of communications methods - secure and insecure. It is a good practice to use secure communications options.

</details>
