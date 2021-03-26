# CRUD REST service

## Links

## Handling HTTP and WebSocket Protocol

### Links
[HTTP](https://nodejs.org/api/http.html)
[HTTPS](https://nodejs.org/api/https.html)
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

How to work with WebSockets in Node.js?

## Middleware. Frameworks. Validation

### Links

### Questions

How to create basic CRUD RESTful service in Node.js?
What is Express and how does it help to create services?
What is a middleware and how it is used in Express?How to setup routing in Express?
How to handle requests and responses in Express?
How to setup a validation in Express? What are the main types of validation?
