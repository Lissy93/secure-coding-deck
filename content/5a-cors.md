With a simple GET fetch request, to an endpoint running under the same domain as your side

![image](https://dev-to-uploads.s3.amazonaws.com/i/qyeikeonofi8dfl0jz2t.gif)

<aside class="notes">
Browsers implement a same-origin policy, which allows a website to freely request data from endpoints under the same origin, but will block websites running under an external URL unless certain conditions are met.

When the browser makes a request, it adds an `Origin: example.com` header to that message. And if that request is going to a server on the same origin, the browser will allow it. 
</aside>
