Notes from my own practice on TryHackMe; not affiliated with or endorsed by TryHackMe.

# Active Directory Security Concepts

This material introduced Active Directory as a centralized identity and access-management service used in many Windows environments. The learning objective was to understand how domains, users, groups, computers, policies, and authentication services fit together. Active Directory supports centralized administration, but excessive privileges and weak configuration can create paths to broad compromise.

Key concepts include directory objects, group membership, Kerberos and LDAP at a conceptual level, service accounts, delegation, and the importance of tiered administration. A security review should focus on effective permissions, privileged group membership, stale accounts, service-account hygiene, and the configuration of domain controllers. Room-specific exploitation steps, credentials, and answers are intentionally excluded.

Defensive controls include least privilege, strong authentication, managed service-account practices, regular review of privileged groups, patching, monitoring authentication anomalies, and protecting domain controllers. I would do differently by documenting the identity relationships and privilege boundaries first, then validating any concern with approved administrative evidence rather than relying on a single tool result.
