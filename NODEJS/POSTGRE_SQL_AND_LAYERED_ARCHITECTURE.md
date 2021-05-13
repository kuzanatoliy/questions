# PostgreSQL and layered architecture

## Links

## Layered Style Guides. Back-End Patterns

### Links
[Organize Node.js API project using 3-layer architecture](https://bytearcher.com/articles/node-project-structure/#:~:text=The%20project%20is%20structured%20into,below%20it%2C%20never%20above%20it.)

### Questions

<details>
  <summary>Why is it pretty good to structure NodeJS application source?</summary>
  
  All of the programmers want to support and increase functionality as easy as possible. One of the main parts of using clean code is using a code structure. So, it is possible to use a lot of ways of code organization. For example, it is possible to organize code by functionality. In this way, to put controller to controllers, server to servers, etc. One more example is an organization by modules. In this way, all functionality depended on users to put the user directory. In my personal opinion, the last one allows splitting functionality to microservices as easy as possible and allows to support more clear file structure.

</details>

<details>
  <summary>What is the 3 Layer approach in the Node.js application?</summary>
  
  It is a base situation when a code structure of a NodeJS application splits into three layers: API, Service and Integration. In this case, each of the layers has a specific responsibility and depends on one below layer.

  API layer:

  The responsibility of the API layer is receiving HTTP requests and parsing payload. Besides, the layer responsible for creating a response. So, this layer gets data and prepares and moves it to the service layer. When it comes back to a result, the layer transforms it, adding HTTP artefacts to a response, for example, express library work on the API layer.

  Service layer:

  The service layer is responsible for performing business logic. So, on the layer, it is needed to implement business requirements and rules. If the layer needs data outside the system, it uses an integration layer. 

  Integration layer:

  The integration layer is responsible for performing I/O outside the application. For example, requests to 3rd party web APIs and talks to databases and file systems.

  In my opinion, using these layers allows using independent unit tests, having a more clean codebase, and doing change into one of the layers without changing others.

</details>

<details>
  <summary>What is the Data Mapper pattern? How is it possible to apply?</summary>
  
  It is one of the programming patterns that splits data(object) and database functionality. The responsibility of the data mapper pattern is communication between the application and database. Moreover, the data objects don't know anything about SQL and are responsible only for their logic.

  Advantages:

  * Each object has its responsibility and is as easy as possible.
  * The logic of the data object and getting/setting data have a weak dependency. As a result mapper or object could be replaced easily.

  Disadvantages:

  * Increase count of entities and code complexity.

</details>

<details>
  <summary>What is a Repository pattern? How is it possible to apply?</summary>

  It is one of the programming patterns. It is a mediator between the data access layer and domain objects.
  Two frequently ways:

  Firstly, Generic Repository. In this case, this pattern is an attempt to abstract from using specific ORM. In my personal opinion, this way is useless because it is impossible to work with the unique functionality of ORM and have to spend additional time to implement versions of the Repository for a few ORM.

  The next one is the Repository as a list of requests to the database.

</details>

## SQL Databases. ORM

### Links
[What a Relational Database is](https://www.oracle.com/database/what-is-a-relational-database/)
[Database normalization](https://en.wikipedia.org/wiki/Database_normalization)
[mssql](https://www.npmjs.com/package/mssql)
[mysql](https://www.npmjs.com/package/mysql2)

### Questions

<details>
  <summary>What is a relational database?</summary>
  
  A relational database is a type of database that stores and provides access to data points. That data is related to one another. The relational model is a base of relational databases, an intuitive, straightforward way of representing data in tables. There each row in the tables is a record with a unique ID called the key. The columns of the table hold attributes of the data, and each record usually has a value, making it easy to establish the relationships among data points.

</details>

<details>
  <summary>What are the main principles of data modelling?</summary>
  
  Data of the database should be not conflicting and understandable. A good database structure should correspond to the 'normal forms'.

  Database normalization is the process of structuring a database, usually a relational database, following a series of so-called 'normal forms' to reduce data redundancy and improve data integrity.

  1NF: The values in each column of a table must be atomic.

  2NF: Each attribute should depend on only the primary key.

  3NF: The table should not have transitive functional dependencies.

</details>

<details>
  <summary>What are the main possibilities/operations of SQL?</summary>
  
  ```SELECT```: getting data from the database.

  ```INSERT```: create a new row into the database table.

  ```UPDATE```: update a row into the database table.

  ```DELETE```: remove a row into the database table.

</details>

<details>
  <summary>How to work with SQL databases using native Node.js driver?</summary>
  
  It is possible to work with a less level package as mysql2 or mssql.

</details>

<details>
  <summary>What is ORM? What are the main ORM concepts?</summary>
  
  Object-relational mapping in computer science is a programming technique for converting data between incompatible type systems using object-oriented programming languages. It creates, in effect, a "virtual object database" that works from within the programming language.

</details>

<details>
  <summary>What is Sequelize ORM?</summary>
  
  Sequelize is a promise-based Node.js ORM for Postgres, MySQL, MariaDB, SQLite and Microsoft SQL Server. It features solid transaction support, relations, eager and lazy loading, read replication and more.

</details>
