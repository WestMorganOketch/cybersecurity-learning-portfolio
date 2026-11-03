# Linux Security and Administration Baseline

Purpose: review a Linux host you administer and identify basic configuration risks.

Useful command patterns
- `id` and `groups` — review the current account and group membership.
- `sudo -l` — review permitted administrative commands for the current account, where authorized.
- `ss -tulpn` — inspect listening network services.
- `systemctl --type=service --state=running` — review running services.
- `journalctl --since '<TIME_WINDOW>'` — inspect system journal events for an approved period.
- `find <APPROVED_PATH> -type f -perm -002` — locate world-writable files within a path you are authorized to audit.

Baseline checks
Review supported package versions, SSH configuration, firewall rules, service exposure, file permissions, scheduled jobs, and local account lifecycle. Confirm that administrative access is limited to approved users and that logs are retained centrally.

Defensive notes
- Apply security updates and remove unused packages.
- Disable unused services and restrict remote administration.
- Use least privilege and separate administrative accounts.
- Protect logs and backups from tampering.
- Monitor failed logins, unexpected privilege changes, and new persistence mechanisms.

Standard reference knowledge added: this sheet uses general Linux administration knowledge because the supplied Linux lab documents were held for private infrastructure indicators; none of their contents were used.
