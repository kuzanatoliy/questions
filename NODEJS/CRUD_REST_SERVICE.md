# CRUD REST service

## Links

## Handling HTTP and WebSocket Protocol

### Links
[HTTP](https://nodejs.org/api/http.html)
[HTTPS](https://nodejs.org/api/https.html)
[WebSockets](https://nodejsdev.ru/doc/websocket/)
[ws](https://www.npmjs.com/package/ws)

### Questions

<details>
  <summary>How to work with HTTP(S) in Node.js?</summary>

  It is possible to used http or https modules for creation servers (createServer) or sending requests. Moreover, when created a server with https need to set an SSL certificate. Also, it is possible to use one of the NodeJS frameworks like Express. It allows more comfortable working with requests.

    var express = require('express');
    var https = require('https');
    var http = require('http');
    var fs = require('fs');
    // This line is from the Node.js HTTPS documentation.
    var options = {
    key: fs.readFileSync('test/fixtures/keys/agent2-key.pem'),
    cert: fs.readFileSync('test/fixtures/keys/agent2-cert.cert')
    }; // Create a service (the app object is just a callback).
    var app = express();
    // Create an HTTP service.
    http.createServer(app).listen(80);
    // Create an HTTPS service identical to the HTTP service.
    https.createServer(options, app).listen(443);

</details>

<details>
  <summary>How to work with WebSockets in Node.js?</summary>

  Firstly about WebSocket. WebSocket is a data transfer protocol. It bases on TCP protocol and allows to send messages between client and server in real-time.
  For the creation of a connection, the client-side sends a request with special headers Upgrade and Connection, and the server-side decides to create or not.
  Both server and client intercept two types of frames:
  
  * data frames;
  * connection frames.
  
  So, It is possible to use WebSockets in NodeJS with external packages as ws or socket.io.

</detauls>

## Middleware. Frameworks. Validation

### Links

### Questions

<details>
  <summary>How to create basic CRUD RESTful service in NodeJS?</summary>

  Firstly, to create and install dependencies for the application.
  Secondly, create one of the variants of the servers(HTTP, HTTPS or HTTP2).
  Next step, creation of an API. Into RESTful API is possible to use HTTP headers and paths for indication of what operation is.
  For example, imagine that we have CRUD RESTful API for working with users profile. In this case, creating the following endpoints:

    GET: /users -> get full list of users;
    GET: /user/{id} -> get user by id;
    POST: /users -> create new one user;
    PUT: /user/{id} -> update user data;
    DELETE: /user/{id} -> delete user;

  So, request artefacts describe what operation will be using. Moreover, it is possible to use one of the NodeJS frameworks like Express, Nest and etc.

</details>

What is Express and how does it help to create services?
What is a middleware and how it is used in Express?
How to setup routing in Express?
How to handle requests and responses in Express?
How to setup a validation in Express?
What are the main types of validation?
