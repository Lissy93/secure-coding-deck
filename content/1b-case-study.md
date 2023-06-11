As we'll see in a bit, this attack and many like it could have been easily prevented if the engineers had followed good security practices.

In this instance<!-- .element: class="fragment" data-fragment-index="1" -->
- **Dependencies**: Being mindful about which dependencies were installed, use of automated security scanning, pinning versions, and a private registry
- **Subresource Integrity (SRI)**: Prevent loading of any resources whose hash doesn't match what you expect it to be
- **Content Security Policy (CSP)**: Prevent loading of third-party data from any domain other than your own
- **Monitoring:** Changes to the website should have been reviewed, monitored and picked up by their anomaly detection system

<!-- .element: class="fragment" data-fragment-index="1" -->

_Although out of the scope for this session, worth also noting that because we cannot control how companies store, use or leak our data, it's important to follow good personal security practices. Notable: Use long, strong and unique passwords, enable 2FA wherever possible, and be mindful about what data you share._
<!-- .element: class="fragment" data-fragment-index="2" -->
