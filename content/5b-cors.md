Now say you've got another website, but it's running under a different domain.
You try and make the same fetch request, but this time it fails with the dreaded CORS error

![image](https://res.cloudinary.com/practicaldev/image/fetch/s--4wGGKnl1--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_66%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/lxhuh29biuwhefs3k9d9.gif)

<aside class="notes">
However if that request is going to a different URL, then it's known as a cross-origin request, and the responding server will add an `Access-Control-Allow-Origin: example.com` header, it's value needs to match the origin header of the request, if not the browser will reject it with a CORS error, preventing the response data from being consumed by the client
</aside>
