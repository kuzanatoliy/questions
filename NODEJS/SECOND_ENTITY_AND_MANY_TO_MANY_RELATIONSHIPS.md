# Second entity and many to many relationships

## Links

## NoSQL Databases. ODM

### Links
[What is NoSQL?](https://aws.amazon.com/nosql/?nc1=h_ls)
[mongodb](https://www.npmjs.com/package/mongodb)
[mongoose](https://www.npmjs.com/package/mongoose)

### Questions

<details>
  <summary>What is a NoSQL database?</summary>

  NoSQL databases are a set of databases that don't use SQL. This concept combines a few types of databases as key-values, documents, graphs, memory.
  NoSQL databases have a great fit for many modern applications such as mobile, web, and gaming that require flexible, scalable, high-performance, and highly functional databases to provide great user experiences.
  Advantages:
  * Flexibility: NoSQL databases provide flexible data structures and enable faster and more iterative development.
  * Scalability: NoSQL databases generally have a design that allows scaling out by using distributed clusters.
  * High-performance: NoSQL databases have great optimization for reading/writing operation.
  * Highly functional: NoSQL databases provide high functionality and data types. Moreover, data models are more understandable because almost the same as the object model.

</details>

<details>
  <summary>What are the main differences between SQL and NoSQL databases?</summary>
  
  For defining differences between SQL and NoSQL databases, needs to compare them by a few points.
  Firstly, optimal workloads:
  Relational databases are designed for transactional and strongly consistent online transaction processing (OLTP) applications and are well for online analytical processing (OLAP).
  The design of NoSQL databases has optimization for many data access patterns that include low-latency applications. And the design of NoSQL search databases has optimizations for analytics over semi-structured data.
  Secondly, Data model:
  The relational model normalizes data into tables that are composed of rows and columns. A schema strictly defines the tables, rows, columns, indexes, relationships between tables, and other database elements. The database enforces the referential integrity in relationships between tables. 
  NoSQL databases provide data models such as key-value, document, and graph. They have optimization for performance and scale.
  Third, Performance:
  SQL databases. Performance is generally dependent on the disk subsystem. The optimization of queries, indexes, and table structure is often required to achieve peak performance.
  NoSQL databases. Performance is generally a function of the underlying hardware cluster size, network latency, and the calling application.
  Forth, Scale:
  Relational databases typically scale up by increasing the compute capabilities of the hardware or scale-out by adding replicas for read-only workloads.
  NoSQL databases usually are partitionable because access patterns can scale out by using distributed architecture to increase throughput that provides consistent performance at a near-boundless scale.
  Last one, APIs:
  Requests to store and retrieve data use queries that conform to a structured query language (SQL). These queries are parsed and executed by the relational database.
  Object-based APIs allow app developers to store and retrieve data structures. Partition keys let apps look up key-value pairs, column sets, or documents that contain serialized app objects and attributes.

</details>

<details>
  <summary>How to work with MongoDB in Node.js using a native driver?</summary>

  It is possible to install the package of the native driver into dependencies.

</details>

What is ODM? What are the main ODM concepts?

<details>
  <summary>How to work with MongoDB in Node.js using Mongoose ODM?</summary>
  
  It is possible to install the package of the Mongoose into dependencies.

</details>

## Asynchronous Network API

### Links

### Questions

How to work with TCP in Node.js?
How does Node.js handle IPC using native modules?
