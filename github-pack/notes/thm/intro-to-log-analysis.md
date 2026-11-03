Notes from my own practice on TryHackMe; not affiliated with or endorsed by TryHackMe.

# Introduction to Log Analysis

This material focused on using logs to understand activity across systems and applications. The objective was to recognize how event records provide evidence for troubleshooting, security monitoring, and incident investigation. Logs become more useful when events from different sources are normalized, timestamped consistently, and viewed in relation to the assets and users involved.

Key concepts include centralized collection, event fields, time zones, filtering, correlation, baselining, and the difference between an isolated event and a meaningful sequence. Analysts should verify the source and integrity of log data, preserve relevant time ranges, and avoid treating a single indicator as conclusive proof. Any example identifiers or challenge answers from the original exercise have been omitted.

Defensive improvements include centralized logging, access controls for log stores, retention policies, alerting on high-risk patterns, and monitoring for gaps in collection. I would do differently by starting with a clear investigative question, recording the time window and data sources, and validating an observation against more than one source before drawing a conclusion.
