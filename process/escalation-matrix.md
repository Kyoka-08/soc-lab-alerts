# SOC Escalation Matrix

| Severity | Example | Acknowledge SLA | Tier 1 Action | Escalate To | Escalation Condition |
|---|---|---|---|---|---|
| Critical | Ransomware signs, domain admin compromise | 15 minutes | Identify host, preserve evidence, investigate immediately | Tier 2 + Incident Response Lead | Immediately |
| High | New admin user, successful brute force | 30 minutes | Check 5W1H and search for the same indicator on other hosts | Tier 2 | If unresolved within 1 hour |
| Medium | Suspicious PowerShell on one host | 4 hours | Investigate using the playbook and verify authorization | Tier 2 if needed | If suspicious activity remains unexplained |
| Low | Internal port scan from a known scanner | 24 hours | Investigate, document, close or tune the rule | None by default | Escalate if evidence indicates malicious activity |

## General Rules

- Acknowledge alerts within the SLA for their severity.
- Prioritize Critical and High alerts.
- Record evidence, investigation steps, verdict and timestamps in each case.
- Escalate when activity is suspicious, unauthorized or unresolved within the defined SLA.
- Do not classify an alert as a confirmed True Positive without sufficient evidence.
