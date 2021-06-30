# CORS (Cross-Origin Resource Sharing)

## Links

### Questions

<details>
  <summary>What is CORS?</summary>

  CORS or Cross-Origin Resource Sharing is a standard that allows clients to get data from third services with different domains using additional HTTP headers.

</details>

<details>
  <summary>What are simple requests?</summary>

  Requests those have the only standard artefacts avoid additional OPTIONS requests. The request should meet the following requirements:

  1. Method: GET, HEAD, or POST;

  2. Has only default user-agent headers as Accept, Accept-Language, Content-Language, Content-Type (Only default types), Last-Event-ID, DPR, Save-Data, Viewport-Width, Width;

  3. The content-Type header should have one of the following values: application/x-www-from-urlencoded, multipart/from-data, text-plain;

  4. The request doesn't have event callbacks for upload events;

  5. The request uses ReadableStream.

</details>
