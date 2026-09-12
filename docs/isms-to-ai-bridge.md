# ISMS → AI agent bridge

For teams that already understand information security management (ISO/IEC 27001-style thinking) and are meeting **agentic AI** for the first time.

This is a translation aid, not a certification mapping or legal advice.

## Familiar control ideas → agent equivalents

| ISMS-style concern | Agent-era equivalent |
| --- | --- |
| Asset inventory | Inventory of models, tools, connectors, and agent identities |
| Access control | What the agent can read/write; tool allowlists; secret handling |
| Segregation of duties | Human approval for high-impact actions; separate deploy vs operate roles |
| Logging and monitoring | Action traces, prompt/tool logs (with redaction), anomaly review |
| Change management | Prompt/tool/config changes treated like code changes |
| Supplier risk | Model vendor, plugin, and SaaS tool diligence |
| Incident management | Agent misuse, runaway actions, data leakage playbooks |
| Business continuity | Kill switch, revoke tokens, fallback to manual process |

## Why 27001 still matters before “AI-only” badges

SMEs and enterprise buyers often trust **information security management** language more than new AI labels. A solid ISMS mindset answers the first buyer questions: who has access, what can change, what is logged, who is accountable.

AI-specific management (e.g. AI management system thinking associated with ISO/IEC 42001) extends that foundation — it does not replace it.

## Practical sequence for a small team

1. Write down what the agent is allowed to do (allowlist).
2. Put humans on the high-impact actions.
3. Keep evidence you would be willing to show a customer or insurer.
4. Only then widen autonomy.

## Related artefacts in this kit

- [agent-control-checklist.md](agent-control-checklist.md)
- [escalation-matrix.md](escalation-matrix.md)
