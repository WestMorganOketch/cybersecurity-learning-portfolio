# SOC Operations and Log Analysis

Purpose: support alert triage and evidence-based investigation.

A reliable investigation begins with a question: what behavior is being explained, during which time window, and on which assets? Identify the relevant data sources, confirm time zones, normalize fields, and correlate events using stable context such as host, account, process, and timestamp. Avoid conclusions based on one event when corroborating evidence is available.

Useful query patterns
- Search a defined time range: `index=<INDEX> earliest=<START_TIME> latest=<END_TIME>`
- Filter for a host: `index=<INDEX> host='<HOST_LABEL>'`
- Group event counts by source: `... | stats count by source`
These are illustrative Splunk-style patterns; adapt field names to the actual data model.

Defensive notes
Centralize logs, restrict access to log stores, retain data according to policy, alert on collection gaps, and document detection logic. Record facts, assumptions, confidence, and escalation decisions separately. Never place credentials or personal data in shared queries or public notes.

Standard reference knowledge added: generic SOC and SIEM guidance; no room flags or answers are reproduced.
