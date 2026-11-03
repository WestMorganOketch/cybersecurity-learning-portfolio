Notes from my own practice on TryHackMe; not affiliated with or endorsed by TryHackMe.

# Windows Forensics Fundamentals

This learning material focused on common Windows artifacts that can help an investigator reconstruct system and user activity. The objective is to understand where evidence may be stored and why it must be interpreted in context. Useful artifact groups include operating-system configuration, user and account information, recent file activity, application execution traces, network profile history, and device connection records.

The important skills are preserving evidence, understanding registry-based artifacts, correlating timestamps, and recognizing that an artifact may be incomplete or affected by normal system behavior. Analysts should record the source, collection method, time zone, and any limitations. This note is based on the supplied general forensics reference; it does not reproduce room answers or a task-by-task walkthrough.

Defensive teams can improve readiness through centralized event collection, endpoint monitoring, time synchronization, controlled retention, and documented evidence-handling procedures. I would do differently by building a repeatable evidence checklist and correlating artifacts with independent event logs before making a conclusion.
