# HTTP

<details>
  <summary>What is a safe http method?</summary>

An HTTP method is safe if it doesn't alter the state of the server. In other words, a method is safe if it leads to a read-only operation. Several common HTTP methods are safe: GET, HEAD, or OPTIONS. All safe methods are also idempotent, but not all idempotent methods are safe. For example, PUT and DELETE are both idempotent but unsafe.

[More >>](https://developer.mozilla.org/en-US/docs/Glossary/Safe/HTTP)

</details>

<details>
  <summary>What is an idempotent method?</summary>

An HTTP method is idempotent if an identical request can be made once or several times in a row with the same effect while leaving the server in the same state. In other words, an idempotent method should not have any side effects — unless those side effects are also idempotent. Implemented correctly, the GET, HEAD, PUT, and DELETE methods are idempotent, but not the POST method. All safe methods are also idempotent.

[More >>](https://developer.mozilla.org/en-US/docs/Glossary/Idempotent)

</details>

<details>
  <summary>What is a cacheable http method?</summary>

A cacheable response is an HTTP response that can be cached, that is stored to be retrieved and used later, saving a new request to the server.

[More >>](https://developer.mozilla.org/en-US/docs/Glossary/cacheable)

</details>

<details>
  <summary>What are HTTP methods? What methods do you know?</summary>

HTTP describes a set of request methods that demonstrate what action is needed. There are the following methods:

`GET` - to request source view. It is possible only to get data;

`HEAD` - the same as the GET but without response;

`POST` - to send subjects to a server and often require changes of the server state or side effects;

`PUT` - to replace all parts of an existed subject;

`PATCH` - to update only part of an existed subject;

`DELETE` - to remove data;

`CONNECT` - to create a connection between server and client;

`OPTIONS` - to get source description;

`TRACE` - to request test a message from a server.

</details>
