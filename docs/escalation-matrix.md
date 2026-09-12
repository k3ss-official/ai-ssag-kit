# Escalation matrix (agent autonomy)

Define when an agent may **proceed**, must **ask**, or must **stop**. Fill owners with real names.

## Decision bands

| Band | Agent behaviour | Example |
| --- | --- | --- |
| **A — Proceed** | Act within allowlist; log evidence | Read a status page; draft an internal summary |
| **B — Ask** | Propose action; wait for human approval | Send external email; change a production setting |
| **C — Stop** | Halt; alert owner | Conflicting instructions; suspected data exfil; policy gap |

## Matrix

| Situation | Band | Approver | Evidence to capture | Recovery |
| --- | --- | --- | --- | --- |
| Tool call on read-only internal data | A | — | query + timestamp | n/a |
| Draft customer-facing message | B | | draft + rationale | edit / discard |
| Spend / purchase / refund | B or C | | amount + vendor + purpose | reverse / dispute |
| Delete / overwrite production data | C | | attempted change | restore backup |
| Credentials or secrets requested | C | | request context | rotate if exposed |
| User asks to bypass policy | C | | verbatim ask | coach + log |
| Model confidence low / conflicting tools | B or C | | uncertainty note | human decide |

## Owners

| Duty | Primary | Backup |
| --- | --- | --- |
| Day-to-day agent owner | | |
| Security escalate | | |
| Business escalate | | |
| Stop-the-line | | |

## Rules of thumb

1. If impact is hard to reverse, default to **Ask** or **Stop**.
2. If the agent cannot explain why an action is allowed, **Stop**.
3. “The model suggested it” is not authority — the matrix is.
