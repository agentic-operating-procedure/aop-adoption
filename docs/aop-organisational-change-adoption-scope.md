# AOP Organisational Change (Adoption Scope)

Informative. This document states the organisational side of the migration: what changes in roles and decision rights, and how the operating culture shifts from corridor execution to exception ownership. The technical migration is the easy half; the estate that fails at adoption fails here.

## 1. The shift

In corridor execution, work moves down a documented path and a person carries it: the person notices what the document missed, improvises the undocumented case, and holds the judgement the document could not write down. In agentic operations, the agent executes the bounded work and the person owns the exceptions: the escalations, the unknown conditions, the drift reviews, the approver rulings.

The shift is not a reduction of people; it is a relocation of judgement. The judgement that used to be spent noticing whether the documented path applies is spent ruling on the cases where the path does not apply, with a complete evidence bundle in hand.

## 2. Roles

| Role | Was | Becomes |
|---|---|---|
| Procedure owner | Author of the SOP, reviewer once a year | Owner of the AOP's intent and scope; rules on boundary changes; owns the risk-axis assessment |
| Approver (per decision class) | The escalation target named in prose ("escalate severe faults") | The named recipient of evidence bundles; rules on cases with rule, provenance and baseline visible; accountable for ruling latency |
| Operator | Corridor executor | Exception owner: works the escalation queue, reviews discrepancies, feeds drift observations |
| Agent supervisor | Does not exist | Owns the harness boundary day to day: fail-closed rates, escalation patterns, credential issuance anomalies |
| Compliance / audit | Samples documents | Audits case records: replays decisions, samples rulings, tests the evidence regime |

## 3. Decision rights

- Decision rights are explicit per decision, stated in the AOP's Authority dimension, and visible to the people who hold them. The single most common adoption failure is a decision class that exists in the AOP but whose named approver did not know they were named.
- Approval latency is a managed metric. An escalation queue that rots converts approval-required into de facto autonomous (agents wait, work stalls, someone widens authority to make the pain stop). The defence is the metric and the roster, not a wider authority.
- Changing authority is a governance event. Any widening of the permitted set or the autonomous class is a new AOP version through the change process, with its risk-axis assessment re-done. The corridor habit of "just this once" is the habit the model exists to end.

## 4. The cultural moves

- **Publish the coverage number.** The documented path's observed coverage (stage 2's finding) is often the most persuasive number in the whole programme. People who have lived the workaround recognize it immediately.
- **Rule on a case, not on a mystery.** Approvers new to evidence bundles distrust them for about two weeks, then do not go back. The bundle must be complete from the first bundle (SEC-9), or trust never forms.
- **Do not measure people by throughput the agent took over.** The operator's new work is exceptions and rulings; the old throughput metric applied to the new role produces gaming. The new metrics are ruling latency, escalation precision and drift response time.
- **Keep the SOP.** The SOP remains the human-readable source of truth the AOP was derived from; its annual review is now informed by the drift record instead of folklore.

## 5. The maturity statement

The organisational change guidance closes where the maturity model opens: an estate states its stage per procedure family, with the evidence, and regresses honestly when a suspension moves a family back. The statement is reviewed with the same cadence as the AOPs themselves.
