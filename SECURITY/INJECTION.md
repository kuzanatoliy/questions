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

<details>
  <summary>What is the ASVS(Application Security Verification Standard)?</summary>

  The ASVS provides a basis for testing web application technical security controls and provides developers with a list of requirements for secure development. The requirements are following objectives in mind:

  * Use as a metric: provide application developers and application owners with a yardstick that allows assessing the degree of trust in your application;

  * Use as guidance: guide security control developers as to what to build into security controls to satisfy application security requirements;

  * Use during procurement: provide a basis for specifying application security verification requirements in contracts.

</details>

<details>
  <summary>What are classes of the SQL injection?</summary>

  Inband(inside): extract data by the same channel as for injection of the SQL code.
  
  Out-of-band(outside): data is retrieved using a different channel.
  
  Inferential or Blind: there is no actual transfer of data, but the tester can reconstruct the information by sending particular requests and observing the resulting behaviour of the DB Server.

</details>

<details>
  <summary>What are SQL injection techniques?</summary>

  It is possible to use five general techniques or their combinations.

  Union Operator: use when the SQL injection flaw happens in a SELECT statement, making it possible to combine two queries into a single result or result set;

  Boolean: use Boolean condition(s) to verify whether certain conditions are true or false;

  Error based: this technique forces the database to generate an error, giving the attacker or taster information which to refine their injection;

  Out-of-band: the technique used to retrieve data using a different channel;

  Time delay: use database commands to delay answers in conditional queries. It is useful when an application doesn't provide results, outputs or errors to an attacker.

</details>
