# Windows Forensics Artifact Reference

Purpose: identify common Windows evidence sources and preserve them in a repeatable, defensible manner.

Artifact areas
- System configuration and operating-system version information.
- Registry hives and control-set configuration.
- User account and profile information.
- Recent file activity and application execution traces.
- Network profile history and connected-device records.
- Event logs and application-specific records.

Collection notes
Preserve original evidence, record acquisition method and time zone, and work from verified copies where possible. Registry artifacts can be affected by system updates and normal use; interpret them with other evidence rather than treating one key as conclusive. Use approved forensic tooling and maintain chain-of-custody records.

Defensive notes
Enable appropriate audit policies, centralize event collection, synchronize system clocks, restrict access to evidence stores, and define retention requirements.

This sheet is based on the supplied general Windows forensics reference and standard knowledge. It contains no screenshots, room answers, user identifiers, or step-by-step room solution.
