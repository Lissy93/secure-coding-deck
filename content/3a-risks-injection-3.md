#### Injection Prevention Rules
- Use prepared statements
- Perform proper input validation - Prefer positive / allowed characters (rather than blocked). Don't rely solely on client-side validation
- Use a safe API - Avoid interacting with services (like a database) directly, but instead build a safe API between the services
- Contextually escape user data - Escape all characters that can be used for malicious things (e.g. `<` for client-side, `"` in databases, etc)
