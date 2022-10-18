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

[More >>](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)

</details>

<details>
  <summary>What is GET method?</summary>

The HTTP GET method requests a representation of the specified resource.

| Option                       | Value |
| ---------------------------- | ----- |
| Request has body             | No    |
| Successful response has body | Yes   |
| Safe                         | Yes   |
| Idempotent                   | Yes   |
| Cacheable                    | Yes   |
| Allowed in HTML forms        | Yes   |

[More >>](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/GET)

</details>

<details>
  <summary>What is HEAD method?</summary>

The HTTP HEAD method requests the headers that would be returned if the HEAD request's URL was instead requested with the HTTP GET method. For example, if a URL might produce a large download, a HEAD request could read its Content-Length header to check the filesize without actually downloading the file.

| Option                       | Value |
| ---------------------------- | ----- |
| Request has body             | No    |
| Successful response has body | No    |
| Safe                         | Yes   |
| Idempotent                   | Yes   |
| Cacheable                    | Yes   |
| Allowed in HTML forms        | No    |

[More >>](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/HEAD)

</details>

<details>
  <summary>What is POST method?</summary>

The HTTP POST method sends data to the server. The type of the body of the request is indicated by the Content-Type header.

| Option                       | Value                                     |
| ---------------------------- | ----------------------------------------- |
| Request has body             | Yes                                       |
| Successful response has body | Yes                                       |
| Safe                         | No                                        |
| Idempotent                   | No                                        |
| Cacheable                    | Only if freshness information is included |
| Allowed in HTML forms        | Yes                                       |

[More >>](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/POST)

</details>

<details>
  <summary>What is PUT method?</summary>

The HTTP PUT request method creates a new resource or replaces a representation of the target resource with the request payload.

| Option                       | Value |
| ---------------------------- | ----- |
| Request has body             | Yes   |
| Successful response has body | May   |
| Safe                         | No    |
| Idempotent                   | Yes   |
| Cacheable                    | No    |
| Allowed in HTML forms        | No    |

[More >>](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/PUT)

</details>
