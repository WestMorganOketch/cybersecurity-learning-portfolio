# Web Application Security

Purpose: connect common web weaknesses to practical prevention and verification.

Review areas
- Authentication: secure sign-in, MFA where appropriate, safe recovery, and session invalidation.
- Authorization: enforce server-side checks for every resource and action.
- Input handling: validate type, length, format, and business rules; encode output for its context.
- Data access: use parameterized queries and least-privileged database accounts.
- Configuration: remove default accounts, debug output, unused endpoints, and exposed backups.
- Dependencies: track versions, apply security updates, and remove unused packages.

Safe verification patterns
- Review application logs for repeated authorization failures and unusual request patterns.
- Use code review and approved scanners in a test environment.
- Confirm that a user cannot access another user's records by changing an identifier. Use synthetic accounts and records only.

Defensive notes
Use prepared statements rather than concatenating untrusted input into SQL. Apply CSRF protection where relevant, secure cookies, content security controls, output encoding, and consistent error handling. Keep secrets in server-side configuration and rotate them if exposure is suspected.

This sheet is conceptual and does not contain exploit payloads or room answers. Standard reference knowledge added for general web security practice.
