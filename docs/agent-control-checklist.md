# Agent control checklist

Use before a pilot where software can **take actions** (send, buy, change, delete, approve, or call tools), not only answer questions.

Mark each item: **Done** / **Partial** / **Missing** / **N/A**.

## 1. Scope

- [ ] Business objective stated in one sentence
- [ ] In-scope systems and data named
- [ ] Explicit out-of-scope list (what the agent must never touch)
- [ ] Success criteria and kill criteria agreed

## 2. Identity and access

- [ ] Agent runs as a dedicated identity (not a shared human login)
- [ ] Least-privilege permissions documented
- [ ] Secrets stored outside prompts / chat logs
- [ ] Access review owner assigned

## 3. Action authority

- [ ] Allowed actions listed (allowlist, not “everything the API offers”)
- [ ] High-impact actions require human approval
- [ ] Rate limits / spend limits set where money or volume is involved
- [ ] Dry-run or shadow mode used before live actions

## 4. Data handling

- [ ] Personal / confidential data classes identified
- [ ] Retention and logging rules defined
- [ ] Redaction rules for prompts, traces, and tickets
- [ ] Third-party model/vendor data path understood

## 5. Oversight and evidence

- [ ] Human owner on call for the pilot window
- [ ] Escalation path tested once
- [ ] Actions logged with who/what/when/why
- [ ] Sample audit trail reviewed by a human

## 6. Failure modes

- [ ] Fail-closed behaviour defined for uncertainty
- [ ] Rollback / revoke plan exists
- [ ] Incident contact and severity levels agreed
- [ ] Stop-the-line authority named

## Sign-off

| Role | Name | Date | Notes |
| --- | --- | --- | --- |
| Business owner | | | |
| Technical owner | | | |
| Security / risk (if required) | | | |
