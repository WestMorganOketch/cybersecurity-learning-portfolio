# Network Inventory and Enumeration

Purpose: build an authorized view of assets, exposed services, and network dependencies. Use only approved address ranges and testing windows.

Common command patterns
- `ip addr` or `ipconfig /all` — inspect local interface configuration.
- `ip route` or `route print` — review local routing information.
- `ss -tulpn` or `netstat -ano` — inspect listening sockets and connections on systems you administer.
- `nmap -sV -oN <OUTPUT_FILE> <AUTHORIZED_TARGET>` — identify reachable services and their versions in an approved assessment. Add conservative timing and explicit scope controls.
- `dig <APPROVED_DOMAIN>` or `nslookup <APPROVED_DOMAIN>` — review DNS records.

Interpretation
A discovered port is not automatically a vulnerability. Validate service ownership, expected exposure, version accuracy, and business need. Record the source, time, scope, and confidence. Avoid scanning third-party or public infrastructure without written authorization.

Defensive notes
- Maintain an asset inventory and approved service baseline.
- Restrict management interfaces to trusted networks.
- Disable unused services and remove stale DNS records.
- Monitor unexpected listeners, inbound connection spikes, and unauthorized network changes.
- Patch exposed services and verify firewall rules against business requirements.

Standard reference knowledge added: command patterns are general administration and assessment references; they are not copied from a room walkthrough.
