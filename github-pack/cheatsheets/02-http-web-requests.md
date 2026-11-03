# HTTP and Web Requests

Purpose: understand client-server communication and safely inspect application behavior.

Common command patterns
- `curl -i https://<AUTHORIZED_HOST>/` — request a resource and display response headers.
- `curl -X GET https://<AUTHORIZED_HOST>/<PATH>` — make a read request.
- `curl -X POST -H 'Content-Type: application/json' --data '<JSON_BODY>' https://<AUTHORIZED_HOST>/<API_PATH>` — submit an approved test payload. Use synthetic data only.
- `curl -I https://<AUTHORIZED_HOST>/` — request headers without retrieving the full body.

Core concepts
HTTP methods describe intended operations; status codes indicate outcomes; headers carry metadata; cookies may maintain session state; content types describe message formats. APIs should enforce authorization on every operation and object, not merely hide controls in the user interface.

Defensive notes
- Use HTTPS and secure cookie attributes.
- Validate and normalize input on the server.
- Apply authentication and object-level authorization consistently.
- Avoid returning stack traces, secrets, or internal details in error responses.
- Log security-relevant events while excluding passwords, tokens, and unnecessary personal data.

Testing notes
Keep requests within scope, use harmless synthetic records, rate-limit tests, and document expected versus observed behavior. A successful response does not prove that access control is correct.

Standard reference knowledge added: generic HTTP and API guidance; examples contain placeholders only.
