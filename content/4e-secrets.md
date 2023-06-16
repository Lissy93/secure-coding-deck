## Secrets Management

Issues with  `.env` files for secret management

- You're storing your secrets in a plaintext file
- Managing several versions (dev, uat, prod, etc) is hard
- You can't (or shouldn't) commit this file to version control, so managing it is hard
- You end up sharing values via insecure means (e.g. docs, Slack, etc)
- There's no way to roll-back or manage versioning
- Impossible to implement secret rotation automatically
- Updating a secret requires a re-deploy
- There's no audit log, to trace back possible breaches

The solution is to use a config server, an external application specifically designed for securely managing keys, secrets, certificates and other sensitive application configuration options.

There's a bunch of options available, like AWS Parameter store, Google Secrets Manager, HashiCorp Vault, etc.

<aside class="notes">
You're probably using `.env` files for secret management, it's what most tutorials recommend you do. But this approach has several issues
</aside>
