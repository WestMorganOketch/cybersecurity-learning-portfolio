Notes from my own practice on TryHackMe; not affiliated with or endorsed by TryHackMe.

# Threat Intelligence Tools

This material explored how open-source intelligence and threat-intelligence services can help analysts assess suspicious domains, URLs, files, and infrastructure. The objective is to understand what different tools contribute and how their results can support an investigation. A reputation score or a single vendor result should be treated as one data point, not a final verdict.

Useful concepts include indicator enrichment, source reliability, context, confidence, false positives, and the difference between tactical indicators and broader threat context. Analysts should compare independent sources, note when information was collected, and avoid submitting confidential or personal data to public services without authorization. Specific exercise answers, indicators, and infrastructure details have been omitted.

Defensively, teams can use threat intelligence to enrich alerts, prioritize investigation, block confirmed malicious indicators, and improve detections. Controls should include review and expiration of blocklists so that stale indicators do not create unnecessary disruption. I would do differently by recording provenance and confidence for each finding and by translating intelligence into a concrete defensive action.
