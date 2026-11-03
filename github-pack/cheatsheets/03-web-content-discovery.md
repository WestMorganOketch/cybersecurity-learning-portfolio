# Web Content Discovery with FFUF

Purpose: understand how authorized content discovery identifies exposed application paths and resources.

Generic pattern
- `ffuf -u https://<AUTHORIZED_HOST>/FUZZ -w <WORDLIST> -mc <STATUS_CODES> -of json -o <OUTPUT_FILE>`
- For a file-extension check, use a controlled extension list such as `<EXTENSION_LIST>` and keep the request rate low.
- Use response-size, status-code, word-count, or line-count filters only after understanding the application's normal responses.

What the options mean
- `FUZZ` marks the request position being varied.
- A wordlist supplies candidate values; quality matters more than volume.
- Match and filter settings help separate expected errors from potentially useful responses.
- Output files support review and reproducibility.

Defensive notes
- Remove obsolete routes, sample files, backups, and exposed administrative resources.
- Require authentication for sensitive functionality.
- Monitor high-volume or unusually patterned requests.
- Apply rate limits and alert on repeated path guessing.
- Ensure error pages do not reveal framework versions or internal paths.

Use only on systems where you have explicit permission. Confirm interesting responses manually and report impact with evidence. Discovery alone is not proof of a vulnerability.

Standard reference knowledge added: this is a generic tool reference, not a room-specific command sequence.
