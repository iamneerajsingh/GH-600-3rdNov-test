
# CityOps Development Decisions

## Decision 001 – Application Architecture

**Decision:** Keep CityOps as a single Flask application.

**Reason:** The workshop focuses on agentic development rather than application architecture complexity.

---

## Decision 002 – Testing

**Decision:** Use unittest.

**Reason:** Keep dependencies minimal.

---

## Decision 003 – Testing Gate

**Decision:** Every behavior change requires automated tests.

**Reason:** Tests provide an objective evaluation signal.


---

## Decision 004 - State

**Decision:** Store task state in `.agent/state.json`.

**Reason:** Agent progress must be represented as a durable artifact.

---

## Decision 005 - Audit

**Decision:** Append audit records to `.agent/audit.jsonl`.

**Reason:** Important agent actions and application events must remain inspectable.

---

## Decision 006 - Security Agent

**Decision:** Security review is read-only.

**Reason:** An independent reviewer should not modify the implementation it is reviewing.