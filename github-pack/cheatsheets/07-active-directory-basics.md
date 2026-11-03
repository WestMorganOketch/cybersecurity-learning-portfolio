# Active Directory Fundamentals

Purpose: understand core directory concepts and review identity security in an authorized Windows domain.

Concepts
- Domains provide a logical identity and administration boundary.
- Users, groups, computers, and service accounts are directory objects.
- Group membership and delegated permissions determine effective access.
- Kerberos and LDAP support authentication and directory access in common deployments.
- Domain controllers are critical infrastructure and require strong protection.

Useful read-only PowerShell patterns (with appropriate administrative modules and permissions)
- `Get-ADDomain` — review domain configuration.
- `Get-ADUser -Filter * -Properties Enabled,LastLogonDate` — review user account status.
- `Get-ADGroupMember -Identity '<GROUP_NAME>'` — inspect group membership.
- `Get-ADDomainController -Filter *` — list domain controllers.

Defensive notes
Review privileged groups, stale accounts, service-account permissions, delegation, password and MFA policy, domain-controller patching, and authentication anomalies. Use tiered administration and separate privileged identities.

Run inventory commands only in domains you administer. Standard reference knowledge added to explain general AD administration; no room-specific attack steps or credentials are included.
