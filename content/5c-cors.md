
CORS has two types of requests: a simple request and a preflighted request. When data is being updated, an extra preflight step is required, to fist ensure that this is allowed.

![preflight](https://dev-to-uploads.s3.amazonaws.com/i/py19auar8xhs933ilmsc.gif)


<aside class="notes">
HTTP requests that involve modifying data (inserting, updating, deleting), like PUT, PATCH and DELETE (or any request with a non-standard header) will need to be pre-flighted. This is where the browser first makes an OPTIONS request to check that the server allows the origin to make a given request with those methods. This then allows the main request to happen afterwards, without fear of disaster. Preflight requests can be cached using the `Access-Control-Max-Age` header, so you don't need to do this for every request (if you need)
</aside>
