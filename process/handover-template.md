# SOC Shift Handover

**Date:** 2026-10-21  
**Environment:** Wazuh lab — Windows-PC  
**Role:** Tier 1 Analyst

## 1. Open Cases

| Issue | Alert | Status | Next Step |
|---|---|---|---|
| #1 | Rule 92201 — PowerShell script creation | Investigating | Verify whether the PowerShell test was authorized |
| #2 | Rule 92201 — PowerShell script creation | Investigating | Compare with Issue #1 and verify the file |
| #3 | Rule 92200 — Microsoft Edge file creation | Investigating | Check whether the activity is normal browser behavior |
| #4 | Rule 92213 — Suspicious PowerShell file | Pending Tier 2 review | Preserve evidence and investigate the script |
| #5 | Rule 92217 — Windows Update executable | Investigating | Verify the executable's signature, hash and source |

## 2. Host Under Observation

- **Host:** Windows-PC
- **IP address:** 192.168.56.109
- Review suspicious PowerShell activity and executable file creation.

## 3. System Issues

- No current system outage has been confirmed.
- Check Wazuh agent connectivity if new alerts indicate the agent has stopped.

## 4. Next Shift Instructions

- Review unresolved Issues #1–#5.
- Record exact acknowledgement and resolution times.
- Verify file paths, process names, signatures and hashes.
- Escalate high-risk activity according to the escalation matrix.
- Do not close cases until investigation is complete.

## 5. Handover Status

All five cases remain open or
