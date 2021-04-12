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

What is Data Mapper pattern and how it could be applied in Node.js application?
What is Repository pattern and how it could be applied in Node.js application?
What is Components approach in Node.js application?

## SQL Databases. ORM

### Links

### Questions

What is a relational database?
What are the main principles of data modeling?
What are the main possibilities/operations of SQL?
How to work with SQL databases using native Node.js driver?
What is ORM? What are the main ORM concepts?How to work with Sequelize ORM?