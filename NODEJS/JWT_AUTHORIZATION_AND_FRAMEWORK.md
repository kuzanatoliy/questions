# JWT authorization and framework

## Authorization. Security. CORS

### Links
[Authentication vs authorization](https://medium.datadriveninvestor.com/authentication-vs-authorization-716fea914d55)
[Passport docs](http://www.passportjs.org/docs/)
[JWT](https://jwt.io/introduction)

### Questions

<details>
  <summary>What are the differences between authentication and authorization?</summary>
  
  A lot of times, authentication and authorization are mixed sentences. But they have differences between each other.

  Authentication is validating user credentials such as username, password, etc. An authenticating system usually identities users by a username and password. Besides, the auth systems could have different elements. Based on the security level, authentication factors can vary from one of the following:
  
  * Single-Factor Authentication: This is the simplest form of authentication method, which requires a password to grant user access to a particular system such as a website or a network. 
  
  * Two-Factor Authentication: This is the most popular and safe authentication type. It requires not only a username and password but also a piece of information only the user knows. 
  
  * Multi-Factor Authentication: This is the most advanced type of authentication, which requires two or more levels of security from independent categories of authentication to grant user access to the system.
  
  Authorization is a process that allows getting access to resources such as files, databases, APIs, etc. So authorization verifies user rights.

</details>

<details>
  <summary>How to set up authentication in the NodeJS service using Passport.js?</summary>
  
  Passport is authentication middleware for Node.js. Extremely flexible and modular. Any application based on express.js can use it. A comprehensive set of strategies support authentication using a username and password, Facebook, Twitter, and more.
  
  So for using, it is possible to install Passport.js and one or more strategies. For more look into documentation.

</details>

<details>
  <summary>What is a JSON Web Token?</summary>
  
  JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

</details>

<details>
  <summary>When should you use JSON Web Tokens?</summary>
  
  It is possible to use JWT for authorization and information exchange:

  * Authorization: It is the most common scenario for using JWT. After the login process, each request will include the JWT, which allows getting access.
  
  * Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed - for example, using public/private key pairs - you can be sure the senders are who they say they are.

</details>

<details>
  <summary>What is the JSON Web Token structure?</summary>
  
  JWT contains three parts:

  * Header. Generally, it has two values: type of the token (JWT), and the signing algorithm, such as HMAC SHA256 or RSA.
  
  * Payload. The part of the token, which contains the claims. There are three types of claims: registered, public, and private.
  
  * Signature. It allows verifying that the message wasn't changed.

</details>

<details>
  <summary>How do JSON web Tokens work?</summary>

  In authentication, when the user successfully logs in using their credentials, the server returns JWT. In general, you should not keep tokens longer than required.

  Whenever the user wants to access a protected route or resource, the user agent should send the JWT, typically in the Authorization header using the Bearer schema.

</details>

What instruments and solutions are used for improving security of Node.js applications?
What is CORS and how does Node.js application can handle it?

## Deploy and Tools

### Links

### Questions

How to deploy Node.js applications on VPS/VDS or other cloud providers?
What tools to use for deployment and maintenance of Node.js application?
