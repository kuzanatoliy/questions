# CRUD REST service

### Links

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

</details>

## Middleware. Frameworks. Validation

### Links
[Express docs](https://expressjs.com)
[Express middlewares](http://expressjs.com/en/guide/using-middleware.html#middleware.application)
[Express validator docs](https://express-validator.github.io/docs/)

### Questions

<details>
  <summary>How to create basic CRUD RESTful service in NodeJS?</summary>

  Firstly, to create and install dependencies for the application.
  
  Secondly, create one of the variants of the servers(HTTP, HTTPS or HTTP2).
  
  Next step, creation of an API. Into RESTful API is possible to use HTTP headers and paths for indication of what operation is.
  
  For example, imagine that we have a CRUD RESTful API for working with users' profiles. In this case, creating the following endpoints:

    GET: /users -> get full list of users;
    GET: /user/{id} -> get user by id;
    POST: /users -> create new one user;
    PUT: /user/{id} -> update user data;
    DELETE: /user/{id} -> delete user;

  So, request artefacts describe what operation will have been using. Moreover, it is possible to use one of the NodeJS frameworks like Express, Nest, etc.

</details>

<details>
  <summary>What is Express? How does it help to create services?</summary>

  Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications. Many popular frameworks use Express as a base of their functionality (NestJS, Kraken, etc.).

  Express allows functionality that manages request processing more comfortable than the native way. Moreover, express has additional libraries that decrease his opportunity, for example, body-parser, etc. Express is effective for working with RESTful API.

</details>

<details>
  <summary>What is middleware? How is it used in Express?</summary>

  Middleware is a function that has access to the request and the response objects and the next middleware function from the application request-response cycle.
  Middleware functions can perform the following tasks:
  
  * Execute any code.
  * Make changes to the request and the response objects.
  * End the request-response cycle.
  * Call the next middleware function in the stack.
  
  An Express application can use the following types of middleware:
  
  Application-level middleware: middleware that works on the application level, for example:
	
    var express = require('express')
	  var app = express()
	  app.use(function (req, res, next) {
  		console.log('Time:', Date.now())
  		next()
	  });
  
  Router-level middleware: middleware that works on the router level, for example:
	  
    var express = require('express')
	  var app = express()
	  var router = express.Router()
	  router.use(function (req, res, next) {
  		  console.log('Time:', Date.now())
  		  next()
	  });
	  app.use(router);

  Error-handling middleware: middleware that has an error object in the arguments, for example:
	
    app.use(function (err, req, res, next) {
  		  console.error(err.stack)
  		  res.status(500).send('Something broke!')
	  });

  Built-in middleware: middleware that moved into external libraries from 4.16.0+ express version, for example, express.static.

  Third-party middleware.

</details>

<details>
  <summary>How to set up routing in express?</summary>
  
  Express has a few functions like .use, .get, .post, etc. that allows setting paths and middlewares.

</details>

<details>
  <summary>How to handle requests and responses in Express?</summary>

  Each middleware has request and response objects and can work with them. Moreover, there is a next callback that allows moving to the next one.

</details>

<details>
  <summary>How to set up validation in Express?</summary>

  It is possible to create middleware that will check data. Moreover, it is possible to use one of the validation libraries. For example, the express-validation library allows using powerful functionality for the creation of effective validation handling.

</details>
