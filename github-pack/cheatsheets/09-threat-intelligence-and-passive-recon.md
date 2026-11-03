# Threat Intelligence and Passive Reconnaissance

Purpose: enrich an investigation using public information and external intelligence sources without over-trusting a single result.

Common patterns
- `whois <APPROVED_DOMAIN>` — review public domain registration information where available.
- `dig <APPROVED_DOMAIN> A` — query DNS records.
- `nslookup <APPROVED_DOMAIN>` — perform a basic DNS lookup.
- Compare a domain, URL, or file indicator across approved intelligence sources; do not upload confidential data to public services without permission.

Analytical practice
Record the source, collection time, confidence, and context for each indicator. Distinguish passive collection from active probing. Consider false positives, shared hosting, stale data, and benign infrastructure before taking action. Public information may still contain personal or sensitive data and should be minimized.

Defensive notes
Use intelligence to enrich alerts, prioritize investigation, detect impersonation, and improve blocklists or detections. Set review and expiry dates for indicators so stale information does not cause unnecessary disruption.

Standard reference knowledge added: general OSINT and threat-intelligence practices; no specific target indicators or platform answers are included.
