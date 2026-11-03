# Windows Security Baseline

Purpose: review a Windows workstation or server using built-in administrative tools.

Useful command patterns
- `whoami /all` — review the current identity, groups, and privileges.
- `Get-ComputerInfo` — collect operating-system and host information.
- `Get-LocalUser` and `Get-LocalGroupMember -Group '<GROUP_NAME>'` — review local accounts and group membership.
- `Get-Service | Where-Object Status -eq 'Running'` — review running services.
- `Get-NetTCPConnection` — inspect active TCP connections.
- `Get-WinEvent -FilterHashtable @{LogName='<LOG_NAME>'; StartTime=(Get-Date).AddDays(-1)}` — review events for a defined time range.

Baseline checks
Review patch status, local administrators, remote access, firewall profiles, endpoint protection, service accounts, startup items, and audit policy. Confirm that logs are time-synchronized and protected from unauthorized modification.

Defensive notes
Use least privilege, strong authentication, application control, supported security updates, and centralized monitoring. Investigate unexpected account creation, privilege assignment, service installation, and remote logon activity.

Standard reference knowledge added: this is general Windows administration guidance; the supplied Windows lab files were excluded because they contained possible private infrastructure details.
